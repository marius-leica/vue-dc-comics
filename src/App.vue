<template>
  <div id="app">
    <TheHeader></TheHeader>
    <section class="jumbo">
      <div class="container position-relative h-100">
        <div
          class="
            current-comics-badge
            bg-primary
            position-absolute
            top-100
            translate-middle
          "
        >
          <span>CURRENT SERIES</span>
        </div>
      </div>
    </section>

    <ComicsCards></ComicsCards>

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
import ComicsCards from "./components/ComicsCards.vue";

export default {
  name: "App",
  components: { TheHeader, BlueBanner, TheFooter, BannerBlack, ComicsCards },
};
</script>

<style lang="scss">
@import "./assets/scss/main.scss";

#app {
  font-family: "Asap Condensed", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.jumbo {
  background-image: url("/public/img/jumbotron.jpg");
  background-size: cover;
  background-position: top;
  background-repeat: no-repeat;
  height: 55vh;
}
.current-comics-badge {
  margin-left: 5%;
  padding: 0.5rem;
  color: white;
  font-size: larger;
}
</style>
