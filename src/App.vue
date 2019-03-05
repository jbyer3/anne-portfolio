<template>
  <div id="app">
    <div id="nav">
      <div class="nav-left">
        <h2>Anne Pengilly</h2>
        <!-- <h2>ANNE PENGILLY</h2> -->
        <h3 id="subz">Collaborative Pianist</h3>
      </div>
      <div class="nav-right">
        <router-link to="/">home</router-link> |
        <router-link to="/about">about</router-link> |
        <router-link to="/recordings">recordings</router-link> |
        <router-link to="/philosophy">philosophy</router-link>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
@import "./public/scss/_colors.scss";
// @import url('https://fonts.googleapis.com/css?family=Roboto');
@import url('https://fonts.googleapis.com/css?family=Pacifico');

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background: $indigo0;
  // color: #2c3e50;
  color: $indigo9;
}
#nav {
  // padding: 30px;
  padding: 0 4rem;
  // background: #a6cbba;
  // background: $cyan4;
  background: $cyan9;
  // color: $lime1;
  color: $indigo0;
  border-bottom: $yellow5 0.3rem solid;
  display: flex;
  justify-content: space-between;
  align-items: center;
  .nav-left {
    font-size: 1.8rem;
    // text-align: left;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    h3 {
      margin: 0 0 0 40px;
      letter-spacing: .04rem;
    }
    h2 {
      margin: 0;
      letter-spacing: .25rem;
      font-family: 'Pacifico', cursive;
    }
  }
  .nav-right {
    a {
      font-weight: bold;
      // color: #2c3e50;
      // color: $gray9;
      color: $indigo0;
      &.router-link-exact-active {
        // color: #42b983;
        color: $yellow5;
      }
    }
  }
}
</style>
