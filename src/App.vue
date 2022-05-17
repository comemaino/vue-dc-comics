<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppShopSection />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppShopSection from "./components/AppShopSection.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppShopSection,
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
  box-sizing: border-box;
}

.container {
  margin: 0 auto;
  width: 80%;
  height: 100%;

  display: flex;
  justify-content: space-between;

  border: 1px solid #0f0;
}
</style>
