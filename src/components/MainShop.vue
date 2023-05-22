<script>
export default {
  name: "MainShop",
  data() {
    return {
      products: [
        {
            img: 'buy-comics-digital-comics.png',
            name: 'Digital Comics',
        },
        {
            img: 'buy-comics-merchandise.png',
            name: 'DC Merchandise',
        },
        {
            img: 'buy-comics-subscriptions.png',
            name: 'Subscription',
        },
        {
            img: 'buy-comics-shop-locator.png',
            name: 'Comic Shop Locator',
        },
        {
            img: 'buy-dc-power-visa.svg',
            name: 'DC Power Visa',
        }
      ],
    };
  },
};
</script>

<template>
  <div class="shop">
    <div class="shop_container">
      <div class="shop_option d-flex" v-for="product in products">
        <img :src="'/img/' + product.img" :alt="product.name" />
        <span>{{product.name.toUpperCase()}}</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>