<script>
export default {
    name: 'ComicsCard',
    props: {
      title: String,
      img: String,
    }
};
</script>

<template>
  <div class="col">
    <div class="my_card">
      <div class="card_img">
        <img :src="img" :alt="title">
      </div>
      <h5>{{ title.toUpperCase() }}</h5>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>