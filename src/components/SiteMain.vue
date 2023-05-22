<script>
import MainShop from "./MainShop.vue";
import MainComics from "./MainComics.vue"

export default {
  name: "SiteMain",
  components: {
    MainShop,
    MainComics
  },
  data() {
    return {
    }
  }
};
</script>

<template>
  <div class="jumbotron"></div>
  <MainComics />
  <MainShop />
</template>

<style lang="scss" scoped></style>