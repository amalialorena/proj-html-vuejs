<template>
  <section>
    <div class="column">
      <div class="title">FEATURED</div>
      <ShopCard
        v-for="(item, i) in featured"
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
        v-for="(item, i) in onSale"
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
        v-for="(item, i) in topRated"
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
        v-for="(item, i) in latestRewiews"
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
  data() {
    return {
      featured: [
        {
          product: "Black Jacket",
          stars: 0,
          discount: "",
          price: "$125",
          img: require("../assets/img/black_leather_jacket-120x156.jpg"),
          by: "",
        },
        {
          product: "Black Jacket",
          stars: 5,
          discount: "$235",
          price: "$200",
          img: require("../assets/img/black_elegant_leather_jacket-120x156.jpg"),
          by: "",
        },
        {
          product: "Black Jacket",
          stars: 0,
          discount: "",
          price: "$57",
          img: require("../assets/img/hipster_black_top-120x156.jpg"),
          by: "",
        },
      ],
      onSale: [
        {
          product: "Black Leather Jacket",
          stars: 5,
          discount: "$235",
          price: "$200",
          img: require("../assets/img/black_elegant_leather_jacket-120x156.jpg"),
          by: "",
        },
        {
          product: "Blue Leather Jacket",
          stars: 5,
          discount: "$80",
          price: "$60",
          img: require("../assets/img/blue_leather_jacket-120x156.jpg"),
          by: "",
        },
        {
          product: "Modern Leather Boots",
          stars: 0,
          discount: "$50",
          price: "$30",
          img: require("../assets/img/modern_leather_boots-120x156.jpg"),
          by: "",
        },
      ],
      topRated: [
        {
          product: "Leather Gloves",
          stars: 5,
          discount: "",
          price: "$45",
          img: require("../assets/img/leather_gloves-120x156.jpg"),
          by: "",
        },
        {
          product: "Black Leather Jacket",
          stars: 5,
          discount: "$235",
          price: "$200",
          img: require("../assets/img/black_elegant_leather_jacket-120x156.jpg"),
          by: "",
        },
        {
          product: "Spring Printed Dress",
          stars: 5,
          discount: "",
          price: "$47",
          img: require("../assets/img/spring_printed_dress-120x156.jpg"),
          by: "",
        },
      ],
      latestRewiews: [
        {
          product: "Black Leather Jacket",
          stars: 5,
          discount: "",
          price: "",
          img: require("../assets/img/black_elegant_leather_jacket-120x156.jpg"),
          by: "by admin",
        },
        {
          product: "Leather Gloves",
          stars: 5,
          discount: "",
          price: "",
          img: require("../assets/img/leather_gloves-120x156.jpg"),
          by: "by Beardman",
        },
        {
          product: "Spring Printed Dress",
          stars: 5,
          discount: "",
          price: "",
          img: require("../assets/img/spring_printed_dress-120x156.jpg"),
          by: "by admin",
        },
      ],
    };
  },
};
</script>


<style scoped lang="scss">
section {
  padding: 20px 0;
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