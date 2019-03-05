<template>
  <div class="page">
    <img src="@/assets/business_card.jpg" alt="business card image">
    <div class="img-text">
      <h1>anne pengilly</h1>
      <h3>{pianist}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "SplashPage"
  // props: {
  //   msg: String
  // }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

img {
  filter: grayscale(0.88);
  width: 63%;
}
</style>
