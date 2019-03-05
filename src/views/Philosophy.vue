<template>
  <div class="about">
    <h1>This is my philosophy page</h1>
    <CallToAction/>
  </div>
</template>

<script>
// @ is an alias to /src
// import Frontpage from '@/components/Frontpage.vue'
import CallToAction from '@/components/CallToAction.vue'


export default {
  name: 'philosophy',
  components: {
    CallToAction
    // Frontpage
  }
}
</script>