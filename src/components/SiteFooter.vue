<script>
import FooterTop from './FooterTop.vue';
import FooterBottom from './FooterBottom.vue';
export default {
  name: "SiteFooter",
  components: {
    FooterTop,
    FooterBottom
  },
  data() {
    return {
    }
    
  }
};
</script>

<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<style lang="scss" scoped></style>