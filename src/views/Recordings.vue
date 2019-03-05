<template>
  <div class="about">
    <h1>This is a recordings page</h1>
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
  name: 'recordings',
  components: {
    Construction
    // CallToAction
    // Frontpage
  }
}
</script>