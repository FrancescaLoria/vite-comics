<script>
import MainTop from "./MainTop.vue";
import MainBottom from "./MainBottom.vue";
export default {
  nome: "AppMain",
  data() {
    return {};
  },
  components: {
    MainTop,
    MainBottom,
  },
};
</script>

<template>
  <main>
    <MainTop />
    <MainBottom />
  </main>
</template>

<style scoped lang="scss"></style>
