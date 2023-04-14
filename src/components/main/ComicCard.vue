<script>
export default {
  name: "ComicCard",
  props: {
    imgUrl: String,
    title: String,
  },
};
</script>

<template>
  <div class="card">
    <img :src="imgUrl" />
    <div class="name-card">{{ title }}</div>
  </div>
</template>

<style scoped lang="scss">
.card {
  width: calc(100% / 6 - 20px);
  margin: 10px;
  color: white;

  img {
    width: 100%;
    height: 150px;
    object-fit: cover;
  }

  .name-card {
    text-transform: uppercase;
    font-size: 12px;
  }
}
</style>
