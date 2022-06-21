<template>
  <div id="app">
    <TheHeader></TheHeader>
    <section class="bg-dark py-5">
      <div class="container"></div>
    </section>
    <BlueBanner></BlueBanner>
    <TheFooter></TheFooter>
    <BannerBlack></BannerBlack>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import BlueBanner from "./components/BlueBanner.vue";
import TheFooter from "./components/TheFooter.vue";
import BannerBlack from "./components/BannerBlack.vue";

export default {
  name: "App",
  components: { TheHeader, BlueBanner, TheFooter, BannerBlack },
};
</script>

<style lang="scss">
@import "assets/scss/main.scss";
@import url("https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;600;700&display=swap");

#app {
  font-family: "Asap Condensed", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
