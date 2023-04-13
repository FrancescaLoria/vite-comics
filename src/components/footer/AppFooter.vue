<script>
import FooterTop from "./FooterTop.vue";
import FooterBottom from "./FooterBottom.vue";
export default {
  nome: "AppFooter",
  data() {
    return {};
  },
  components: {
    FooterTop,
    FooterBottom,
  },
};
</script>

<template>
  <FooterTop />
  <FooterBottom />
</template>

<style scoped lang="scss"></style>
