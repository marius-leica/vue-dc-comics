<template>
  <div>
    <nav class="navbar navbar-expand-lg bg-light">
      <div class="container d-flex justify-space-betwen">
        <a class="navbar-brand" href="#">
          <img src="/img/dc-logo.png" alt="" width="50" height="50" />
        </a>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
            <li class="nav-item" v-for="link in navLinks" :key="link">
              <a class="nav-link active" aria-current="page" href="#">{{
                link
              }}</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
  data() {
    return {
      navLinks: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
      //
    };
  },
  components: {},
};
</script>

<style lang="scss" scoped>
a.nav-link:hover {
  color: blue;
  border-bottom: 1px solid blue;
}
</style>