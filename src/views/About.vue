<template>
  <div class="about">
    <h1>This is an about page</h1>
    <Biography/>
    <CallToAction/>
  </div>
</template>

<script>
// @ is an alias to /src
// import Frontpage from '@/components/Frontpage.vue'
import CallToAction from '@/components/CallToAction.vue'
import Biography from '@/components/Biography.vue'

export default {
  name: 'about',
  components: {
    CallToAction,
    Biography
    // Frontpage
  }
}
</script>