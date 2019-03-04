<template>
  <div class="about">
    <h1>This is my philosophy page</h1>
    <Frontpage/>
  </div>
</template>

<script>
// @ is an alias to /src
import Frontpage from '@/components/Frontpage.vue'

export default {
  name: 'philosophy',
  components: {
    Frontpage
  }
}
</script>