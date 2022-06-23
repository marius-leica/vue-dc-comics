<template>
  <div>
    <div class="card-comic">
      <div class="comic-img">
        <img :src="urlImg" :alt="`Cover image of ${comicTitle} `" />
      </div>
      <div class="comic-text py-2 text-start text-light">
        <span class="card-title pb-3 text-uppercase">
          {{ comicTitle }}
        </span>
      </div>
      <div class="card-overlay p-5 d-flex flex-column">
        <div><strong>price: </strong>{{ comicPrice }}</div>
        <div><strong>format: </strong>{{ comicType }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingleCard",
  props: {
    urlImg: String,
    comicTitle: String,
    comicPrice: String,
    comicType: String,
  }
};


</script>

<style lang="scss" scoped>
.card-comic {
  position: relative;
  margin-bottom: 0.5rem;

  &:hover {
    box-shadow: 0px 0px 10px #000;
    transition: all 0.3s ease-in-out;

    .card-overlay {
      opacity: 0.8;
    }
  }
}

.card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
  background-color: rgba($color: #000000, $alpha: 1.0);
  color: white;
}

.comic-img {
  aspect-ratio: 1/1;
  overflow: hidden;
}
</style>