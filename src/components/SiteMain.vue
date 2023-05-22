<script>
import MainShop from "./MainShop.vue";
import ComicsCard from "./ComicsCard.vue";
import comics from "../data/dc-comics.json"

export default {
  name: "SiteMain",
  components: {
    MainShop,
    ComicsCard
  },
  data() {
    return {
      comics: comics
    }
  }
};
</script>

<template>
  <div class="jumbotron"></div>
  <div class="main_content">
    <ComicsCard />
  </div>
  <MainShop />
</template>

<style lang="scss" scoped></style>