<template>
  <div class="comic-card">
    <div class="img-wrapper">
      <img :src="comicCard.thumb" alt="" />
    </div>
    <h4>{{ comicCard.series }}</h4>
  </div>
</template>

<script>
export default {
  name: "AppComicCard",

  props: {
    comicCard: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../components/style/common.scss";

.comic-card {
  width: calc(100% / 6 - 2rem);

  .img-wrapper {
    width: 100%;
    aspect-ratio: 1;
    overflow: hidden;

    img {
      width: 100%;
    }
  }
  h4 {
    margin: 1rem 0;
    text-transform: uppercase;
  }
}
</style>
