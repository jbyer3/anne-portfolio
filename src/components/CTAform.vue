<template>
<form>
  <p>
    <label>
      Your Name: <input type="text" name="name" v-model="form.name" />
    </label>
  </p>
  <p>
    <label>
      Your Email: <input type="email" name="email" v-model="form.email" />
    </label>
  </p>
  <p>
    <label>
      Your Phone: <input type="text" name="phone" v-model="form.phone" />
    </label>
  </p>
  <p>
    <label>
      Message: <textarea name="message" v-model="form.message" />
    </label>
  </p>
  <p>
    <button type="submit" @click.prevent="handleSubmit">Send</button>
  </p>
</form>
</template>


<script>
export default {
  data() {
    return {
      form: {
        name: '',
        email: '',
        phone: '',
        message: '',
      },
    };
  },
  methods: {
    encode(data) {
      return Object.keys(data)
        .map(
          key => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`
        )
        .join('&');
    },
    handleSubmit() {
      fetch('/', {
        method: 'POST',
        headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
        body: this.encode({ 'form-name': 'contact', ...this.form }),
      })
        .then(() => alert('Success!'))
        .catch(error => alert(error));
    },
  },
};
</script>

<style lang="scss" scoped>
.page {
  display: flex;
  flex-direction: column;
  align-items: center;
}

form {
  width: 20rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  // width: 30rem;
}

label {
  flex-shrink: 1;
  margin-right: 2rem;
}

.form-item {
  margin: 0.2rem;
  // padding: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  flex-wrap: nowrap;
  width: 70%;
  .text-inputs {
    font-size: 1.2rem;
    border-radius: 0.2em;
    height: 120%;
  }
}
</style>