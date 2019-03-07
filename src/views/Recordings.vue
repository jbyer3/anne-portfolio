<template>
  <div class="about">
    <h1>This is a recordings page</h1>
    <!-- <Construction/> -->
    <CallToAction/>
  </div>
</template>

<script>
// @ is an alias to /src
// import Construction from '@/components/Construction.vue'
// import SplashPage from '@/components/SplashPage.vue'
import CallToAction from '@/components/CallToAction.vue'

export default {
  name: 'recordings',
  components: {
    // Construction,
    // SplashPage,
    CallToAction
  }
}
</script>