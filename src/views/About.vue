<template>
  <div class="about">
    <h1>This is an about page</h1>
    <Biography/>
    <CallToAction/>
    <!-- <Construction/> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import Construction from '@/components/Construction.vue'
import CallToAction from '@/components/CallToAction.vue'
import Biography from '@/components/Biography.vue'

export default {
  name: 'about',
  components: {
    // Construction
    Biography,
    CallToAction
  }
}
</script>