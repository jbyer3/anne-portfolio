<template>
  <div class="home">
    <h1>homepagio</h1>
    <SplashPage/>
    <CTAform/>
    <!-- <CallToAction/> -->
    <!-- <Construction/> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import Construction from '@/components/Construction.vue'
import SplashPage from '@/components/SplashPage.vue'
import CTAform from '@/components/CTAform.vue'
// import CallToAction from '@/components/CallToAction.vue'

export default {
  name: 'home',
  components: {
    // Construction,
    SplashPage,
    CTAform
    // CallToAction
  }
}
</script>
