<template>
  <div id="app">
    <AppHeader />
    <AppBanner />
    <AppMain />
    <AppShopSection />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppBanner from "./components/AppBanner.vue";
import AppMain from "./components/AppMain.vue";
import AppShopSection from "./components/AppShopSection.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppBanner,
    AppMain,
    AppShopSection,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./components/style/common.scss";
</style>
