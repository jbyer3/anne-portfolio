<template>
  <div class="page">
    <div class="call-to-action">
      <h1>Contact me for a gig</h1>
      <form action="/">
        <div class="form-item">
          <label for="name">Name</label>
          <input type="text" name="name" id="name">
        </div>
        <div class="form-item">
          <label for="email">Email</label>
          <input type="email" name="email" id="email">
        </div>
        <div class="form-item">
          <label for="phone-number">phone</label>
          <input type="text" name="phone-number" id="phone-number">
        </div>
        <div class="form-item">
          <label for="cta-message">Name!</label>
          <textarea type="text" name="cta-message" id="cta-message"></textarea>
        </div>
      </form>
    </div>
  </div>
</template>

<style lang="scss" scoped>
// html, body {
//   padding: 0;
//   margin: 0;
//   box-sizing: border-box;
//   font-family: 'Roboto', sans-serif;
//   background: #dad8f3;

// }

// a {
//   text-decoration: none;
//   color: rgb(84, 137, 203);

// }

// a:hover {
//   color: rgb(213, 85, 187)
// }

// .page {
//   display: flex;
//   flex-direction: column;
//   align-items: center;
// }

.call-to-action form {
  display: flex;
  flex-direction: column;
}

.form-item * {
  margin: 0;
  padding: 0;
}
</style>


