<template>
  <main id="main">
    <div class="container">
      <h1 class="title">Content goes here</h1>
    </div>
  </main>
</template>

<script>
export default {
  name: "AppMain",
};
</script>

<style lang="scss" scoped>
@import "../components/style/common.scss";
#main {
  height: 100px;
  line-height: 100px;
  color: #fff;
  background-color: #222;
}
</style>
