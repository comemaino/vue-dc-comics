<template>
  <div class="banner">
    <div>Current Series</div>
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

  div {
    padding: 0.8rem;
    color: #fff;
    background-color: #18f;
    font-weight: 700;
    text-transform: uppercase;

    position: absolute;
    bottom: -1.4rem;
    left: 11rem;
  }
}
</style>
