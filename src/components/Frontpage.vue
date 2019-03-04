<template>
  <div>
  <div class="nav">
    <div class="nav-left">
      <h1 id="hero-name">anne pengilly</h1>
      <h4>collaborative pianist</h4>
    </div>
    <div class="nav-right">
      <a href=""><h3>about me</h3></a>
      <a href=""><h3>recordings</h3></a>
      <a href=""><h3>info?</h3></a>
    </div>
  </div> 
  <div class="page">
    <div class="photo-placeholder">
    </div>

    <div class="testimonials">
      <div class="testimonial testimonial-one">
        dis mah blurp one
      </div>
      <!-- <div class="testimonial testimonial-two">
        dis mah blurp two
      </div>
      <div class="testimonial testimonial-three">
        dis mah blurp three
      </div>
      <div class="testimonial testimonial-four">
        dis mah blurp four
      </div>
      <div class="testimonial testimonial-five">
        dis mah blurp five
      </div>
      <div class="testimonial testimonial-six">
        dis mah blurp six
      </div>
      <div class="testimonial testimonial-seven">
        dis mah blurp seven 
      </div>
      <div class="testimonial testimonial-eight">
        dis mah blurp eight
      </div>
      <div class="testimonial testimonial-nine">
        dis mah blurp nine
      </div> -->

      <div class="call-to-action">
        <form action="/">
          <div class="form-item">
            <label for="name">Name!</label>
            <input type="text" name="name" id="name">
          </div>
          <div class="form-item">
            <label for="email">Email!</label>
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
  </div>
  </div>
</template>

<style lang="scss" scoped>
html, body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
  background: #dad8f3;

}

a {
  text-decoration: none;
  color: rgb(84, 137, 203);

}

a:hover {
  color: rgb(213, 85, 187)
}

.nav {
  width: 100%;
  height: 8rem;
  background: rgb(33, 48, 67);
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: rgb(84, 137, 203);
  position: sticky;
  top: 0;
}

#hero-name {
  font-size: 4rem;
  /* color: rgb(84, 137, 203); */
}

.nav-left * {
  padding: 0;
  margin: 0;
}

.nav .nav-left {
  margin-top: 0;
  margin-left: 8rem;
  font-family: 'Lobster', cursive;
  font-size: 2rem;
}

.nav .nav-right {
  display: flex;
  justify-content: flex-end;
  margin-right: 4rem;
}

.nav-right * {
  margin-right: 1rem;
}

.menu-dropdown {
  display: flex;
  justify-content: flex-end;
  margin-right: 5rem;
}

.page {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.photo-placeholder {
  height: 40rem;
  width: 50rem;
  background: white;
}

.testimonials *{
  margin: 2rem;
}

.call-to-action form {
  display: flex;
  flex-direction: column;
}

.form-item * {
  margin: 0;
  padding: 0;
}
</style>


