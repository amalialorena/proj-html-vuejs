<template>
  <div :class="`card ${customClass ? customClass : ''}`">
    <div class="product">
      <span class="product-name">{{ productName }}</span>
      <div v-if="stars ? 'stars' : ''" class="stars">
        <span v-for="index in stars" :key="index">&#9733;</span>
      </div>
      <span v-if="discount ? 'discount' : ''" class="discount"
        ><s>{{ discount }}</s></span
      >
      <span class="price" :class="discount ? 'underline' : ''">{{
        price
      }}</span>
      <div v-if="by ? 'by' : ' '" class="by">{{ by }}</div>
    </div>
    <div class="img-container">
      <img :src="img" />
    </div>
  </div>
</template>

<script>
export default {
  name: "ShopCard",
  props: {
    productName: String,
    stars: Number,
    discount: String,
    price: String,
    by: String,
    img: String,
    customClass: String,
  },
};
</script>

<style scoped lang="scss">
.card {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #f4f4f4;
  padding-bottom: 10px;
  color: #585758;
  margin-bottom: 10px;

  &.footer {
    color: white;
    border-bottom: 1px solid #444;

    .product {
      .discount,
      .price {
        color: white;
      }
    }
  }

  .product {
    .product-name {
      font-weight: bold;
      font-size: .9em;
    }
    .stars {
      color: #427ed1;
      font-size: 14px;
    }
    .price {
      color: black;
      font-weight: 700;
      margin: 0 3px;
    }
    .discount {
      color: black;
      font-weight: 700;
    }
    .underline {
      text-decoration: underline;
    }
  }
  .img-container {
    height: 80px;
    img {
      height: 100%;
    }
  }
}
</style>