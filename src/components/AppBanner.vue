<template>
  <div class="banner">
    <div class="button">Current Series</div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../components/style/common.scss";

.banner {
  height: 400px;
  background-image: url(../assets/img/jumbotron.jpg);

  position: relative;

  .button {
    position: absolute;
    bottom: -1.4rem;
    left: 11rem;
  }
}
</style>
