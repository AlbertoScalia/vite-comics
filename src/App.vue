<script>
export default {
  data() {
    return {
      message: "Helloo",
    };
  },
};
</script>

<template>
<div class="my-container debug">
  <header>
    <div class="header_container"></div>
  </header>
  
  <main>
    <div class="main_content">
      <div class="content_container">--&gt; Content goes here &lt;--</div>
    </div>
    <div class="shop">
      <div class="shop_container"></div>
    </div>
  </main>
  
  <footer>
    <div class="footer_top">
      <div class="top_container">
        <div class="my_col"></div>
        <div class="my_col"></div>
        <div class="my_col"></div>
      </div>
    </div>
    
    <div class="footer_bottom">
      <div class="bottom_container">
        <div class="bottom_left"></div>
        <div class="bottom_right">

        </div>
      </div>
    </div>
  </footer>
</div>
</template>

<style lang="scss" scoped>
.debug header {
  height: 80px;
  background-color: red;
}

.debug .footer_top {
  height: 280px;
  background-color: grey;
    .my_col {
      height: 100%;
      background-color: red;
      border: 1px dashed;
      width: calc(100% / 10);
    }
}

.debug .footer_bottom {
  .bottom_container {
    justify-content: space-between;
  }
  height: 80px;
  background-color: /* dark */ darkblue;
  .bottom_left {
    width: calc(100% / 9);
    border: 1px dashed yellow;
  }
  .bottom_right {
    width: calc(100% / 3);
    border: 1px dashed yellow;
  }
}
</style>