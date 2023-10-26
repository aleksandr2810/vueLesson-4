<template>
  <div class="container">
    <div class="img">
      <img :src="cardData.imgSrc" class="img" />
    </div>
    <div class="title">
      <a :href="cardData.link">
        {{ cardData.title }}
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FavoriteCard',

  props: {
    cardData: {
      type: Object,
      default: () => ({}),
    },
  },
}
</script>

<style lang="css" scoped>
.container {
  display: inline-block;
  width: 80px;
  height: 150px;
  border: 2px solid green;
  border-radius: 12px;
}
.img {
  width: 80px;
  height: 130px;
}
.title {
  color: blueviolet;
}
</style>
