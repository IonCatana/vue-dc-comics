<template>
  <div id="app">
    <MyHeader />
    <MyMain />
    <MyBannerBlu />
    <MyFooter />
    <MyFooterNavBar />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyMain from "./components/MyMain.vue";
import MyFooter from "./components/MyFooter.vue";
import MyBannerBlu from "./components/MyBanner.vue";
import MyFooterNavBar from "./components/MyFooterNavBar.vue";
export default {
  name: "App",
  components: {
    MyHeader,
    MyMain,
    MyBannerBlu,
    MyFooter,
    MyFooterNavBar,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
