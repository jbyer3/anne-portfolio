<template>
  <div class="page">
    <div class="call-to-action">
      <h1>Contact me for a gig</h1>
      <form name="contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field">
        <div class="form-item">
          <label for="name">name:</label>
          <input class="text-inputs" type="text" name="name" id="name">
        </div>
        <div class="form-item">
          <label for="email">email:</label>
          <input class="text-inputs" type="email" name="email" id="email">
        </div>
        <div class="form-item">
          <label for="phone-number">phone:</label>
          <input class="text-inputs" type="text" name="phone-number" id="phone-number">
        </div>
        <div class="form-item">
          <label for="cta-message">message:</label>
          <textarea class="text-inputs" type="text" name="cta-message" id="cta-message" rows="15"></textarea>
        </div>
        <button type="submit">send me an email</button>
      </form>
    </div>
  </div>
</template>

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


