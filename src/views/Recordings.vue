<template>
  <div class="about">
    <h1>This is a recordings page</h1>
    <Frontpage/>
  </div>
</template>

<script>
// @ is an alias to /src
import Frontpage from '@/components/Frontpage.vue'

export default {
  name: 'recordings',
  components: {
    Frontpage
  }
}
</script>