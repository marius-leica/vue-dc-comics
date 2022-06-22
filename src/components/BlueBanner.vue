<template>
  <div class="bg-primary py-5">
    <div class="container">
      <ul class="list-unstyled d-flex justify-content-between">
        <li
          v-for="(link, i) in blueBannerLinks"
          :key="i"
          class="d-flex align-items-center"
        >
          <img :src="link.url" alt="" width="40px" height="50px" />
          <a
            class="nav-link active ms-1 text-light"
            aria-current="page"
            href="#"
            >{{ link.link }}</a
          >
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BlueBanner",
  data() {
    return {
      blueBannerLinks: [
        {
          url: "/img/buy-comics-digital-comics.png",
          link: "DIGITAL COMICS",
        },
        {
          url: "/img/buy-comics-merchandise.png",
          link: "DC MERCHANDISE",
        },
        {
          url: "/img/buy-comics-subscriptions.png",
          link: "SUBSCRIPTION",
        },
        {
          url: "/img/buy-comics-shop-locator.png",
          link: "COMIC SHOP LOCATOR",
        },
        {
          url: "/img/buy-dc-power-visa.svg",
          link: "DC POWER VISA",
        },
      ],
      //
    };
  },
  components: {},
};
</script>

<style lang="scss">
</style>
