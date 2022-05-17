<template>
  <div id="app">
    <AppHeader />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

* {
  margin: 0;
  padding: 0;
  // box-sizing: border-box;
}

.container {
  margin: 0 auto;
  width: 80%;
  height: 100px;
  display: flex;
  justify-content: space-between;

  border: 1px solid #000;
}
</style>
