<style src="./ProductGallery.scss" lang="scss" scoped></style>
<script src="./ProductGallery.js"></script>

<template>
  <div v-if="product" class="pro-dec-big-img-slider product-big-img-style">
    <div class="easyzoom easyzoom--overlay" ref="easyzoom">
      <a :href="productImage">
        <img
          :class="!quickview ? 'product-image' : 'quickview-img'"
          :src="productImage"
          alt=""
          data-test="product-image"
        />
      </a>
    </div>
    <!-- <div class="pro-dec-zoom-img">
      <a class="img-popup" :href="productImage"><i class="fa fa-search-plus"></i></a>
    </div>-->
    <!-- <div class="product-dec-slider product-small-img-style mt-10">
    <div class="product-dec-small active">
      <img src="assets/images/product-details/small-1.jpg" alt="">
    </div>
    <div class="product-dec-small">
      <img src="assets/images/product-details/small-2.jpg" alt="">
    </div>
    <div class="product-dec-small">
      <img src="assets/images/product-details/small-3.jpg" alt="">
    </div>
    <div class="product-dec-small">
      <img src="assets/images/product-details/small-4.jpg" alt="">
    </div>
    <div class="product-dec-small">
      <img src="assets/images/product-details/small-2.jpg" alt="">
    </div>
    </div>-->
  </div>
</template>
