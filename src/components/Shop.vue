<template>
  <section>
    <div class="column">
      <div class="title">FEATURED</div>
      <ShopCard
        v-for="(item, i) in products.featured"
        :key="i"
        :productName="item.product"
        :img="item.img"
        :price="item.price"
        :stars="item.stars"
        :by="item.by"
        :discount="item.discount"
      />
    </div>
    <div class="column">
      <div class="title">ON SALE</div>
        <ShopCard
        v-for="(item, i) in products.onSale"
        :key="`onSale-${i}`"
        :productName="item.product"
        :img="item.img"
        :price="item.price"
        :stars="item.stars"
        :by="item.by"
        :discount="item.discount"
      />
  </div>
  <div class="column">
      <div class="title">TOP RATED</div>
        <ShopCard
        v-for="(item, i) in products.topRated"
        :key="`topRated-${i}`"
        :productName="item.product"
        :img="item.img"
        :price="item.price"
        :stars="item.stars"
        :by="item.by"
        :discount="item.discount"
      />
  </div>
  <div class="column">
      <div class="title">LATEST REWIEWS</div>
        <ShopCard
        v-for="(item, i) in products.latestRewiews"
        :key="`latestRewiews-${i}`"
        :productName="item.product"
        :img="item.img"
        :price="item.price"
        :stars="item.stars"
        :by="item.by"
        :discount="item.discount"
      />
  </div>
  </section>
</template>

<script>
import ShopCard from "../components/ShopCard.vue";
export default {
  name: "Shop",
  components: {
    ShopCard,
  },
  props: {
    products: {
      featured: Array,
      onSale: Array,
      topRated: Array,
      latestRewiews: Array,
    },
  }
};
</script>


<style scoped lang="scss">
section {
  padding: 50px 0;
  width: 70%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  min-width: 1100px;
  .column {
    margin: 10px;
    width: 100%;
    .title {
      font-size: 0.9em;
      color: #413f41;
      margin: 10px 0;
    }
  }
}
</style>