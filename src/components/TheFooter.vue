<template>
  <div class="footer-bg py-4">
    <div class="container">
      <div class="row">
        <div class="col-md-2 text-start">
          <h5 class="text-light">DC COMICS</h5>
          <ul class="list-unstyled">
            <li
              class="text-light text-start"
              v-for="(link, i) in dcComics"
              :key="link"
            >
              <span>{{ dcComics[i] }}</span>
            </li>
          </ul>
          <h5 class="text-light">SHOP</h5>
          <ul class="list-unstyled">
            <li
              class="text-light text-start"
              v-for="(link, i) in shop"
              :key="link"
            >
              <span>{{ shop[i] }}</span>
            </li>
          </ul>
        </div>
        <div class="col-md-2 text-start">
          <h5 class="text-light">DC</h5>
          <ul class="list-unstyled text-start">
            <li class="text-light" v-for="(link, i) in dc" :key="link">
              <span>{{ dc[i] }}</span>
            </li>
          </ul>
        </div>
        <div class="col-md-2 text-start">
          <h5 class="text-light">SITES</h5>
          <ul class="list-unstyled">
            <li
              class="text-light text-start"
              v-for="(link, i) in sites"
              :key="link"
            >
              <span>{{ sites[i] }}</span>
            </li>
          </ul>
        </div>
        <div class="col-md-6">
          <img src="/img/dc-logo-bg.png" alt="" height="400px" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheFooter",
  data() {
    return {
      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      shop: ["Shop DC", "Shop DC Collectibles"],
      dc: [
        "Terms of Use",
        "Privacy Policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],

      //
    };
  },
};
</script>

<style lang="scss" scoped>
.footer-bg {
  background-image: url("/public/img/footer-bg.jpg");
}
li span {
  font-size: 0.8rem;

  &:hover {
    text-decoration: underline;
    cursor: pointer;
  }
}
</style>