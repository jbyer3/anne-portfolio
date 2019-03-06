<template>
  <div class="home">
    <h1>homepagio</h1>
    <SplashPage/>
    <CallToAction/>
    <!-- <Construction/> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import Construction from '@/components/Construction.vue'
import SplashPage from '@/components/SplashPage.vue'
import CallToAction from '@/components/CallToAction.vue'

export default {
  name: 'home',
  components: {
    // Construction,
    SplashPage,
    CallToAction
  }
}
</script>
