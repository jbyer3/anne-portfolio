<template>
  <div id="app">
    <div id="nav">
      <div class="nav-left">
        <h2>Anne Pengilly</h2>
        <h3>collaborative pianist</h3>
      </div>
      <div class="nav-right">
        <router-link to="/">Home</router-link>|
        <router-link to="/about">About</router-link>|
        <router-link to="/recordings">Recordings</router-link>|
        <router-link to="/philosophy">Philosophy</router-link>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  // padding: 30px;
  padding: 0 4rem;
  background: #a6cbba;
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
      margin: 0;
      letter-spacing: .04rem;
    }
    h2 {
      margin: 0;
      letter-spacing: .25rem;
    }
  }
  .nav-right {
    a {
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
}
</style>
