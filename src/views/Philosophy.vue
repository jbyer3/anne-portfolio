<template>
  <div class="about">
    <h1>This is my philosophy page</h1>
    <!-- <CallToAction/> -->
    <Construction/>
  </div>
</template>

<script>
// @ is an alias to /src
// import Frontpage from '@/components/Frontpage.vue'
// import CallToAction from '@/components/CallToAction.vue'
import Construction from '@/components/Construction.vue'


export default {
  name: 'philosophy',
  components: {
    Construction
    // CallToAction
    // Frontpage
  }
}
</script>