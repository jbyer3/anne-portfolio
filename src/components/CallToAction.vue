<template>
  <div class="page">
    <div class="call-to-action">
      <h1>Contact me for a gig</h1>
      <form action="/" name="contact" method="post" data-netlify="true" data-netlify-honeypot="bot-field">
        <input type="hidden" name="form-name" value="contact" />
        <label for="name">name:</label>
        <input class="text-inputs" type="text" name="name" id="name" required>
        <label for="email">email:</label>
        <input class="text-inputs" type="email" name="email" id="email" required>
        <label for="phoneNumber">phone:</label>
        <input class="text-inputs" type="text" name="phoneNumber" id="phoneNumber">
        <label for="ctaMessage">message:</label>
        <textarea class="text-inputs" type="text" name="ctaMessage" id="ctaMessage" rows="15" required></textarea>
        <button type="submit">send me an email</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CallToAction',
  data: () => ({
    form: {
      contact: ""
    }
  }),
  methods: {
    // encode(data) {
    //   return Object.keys(data)
    //     .map(
    //       key => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`
    //     )
    //     .join("&")
    // },
    // handleSubmit() {
    //   const axiosConfig = {
    //     header: { "Content-Type": "application/x-www-form-urlencoded" }
    //   };
    //   axios.post(
    //     "/",
    //     this.encode({
    //       "form-name": "contact",
    //       ...this.form
    //     }),
    //     axiosConfig
    //   );
    // },
    // onSubmit: (e)=> {
    //   console.log(e.srcElement.elements)
    //   const { name, phoneNumber, email, ctaMessage } = e.srcElement.elements;
    //   console.log('name is: ', name.value)
    //   console.log('phoneNumber is: ', phoneNumber.value)
    //   console.log('email is: ', email.value)
    //   console.log('ctaMessage is: ', ctaMessage.value)
    // }
  }
}
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


