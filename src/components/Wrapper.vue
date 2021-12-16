<template>
  <div>
    <Nav />
    <Header />
    <FeaturedProducts />
    <Collections />
    <BestSeller />
    <Offers />
    <NewArrivals />
    <Quotes />
    <Blog />
    <Shop :products="products" />
    <Brands />
    <Footer :products="products.topRated"/>
  </div>
</template>

<script>
import Nav from "./nav/Nav.vue";
import Header from "../components/Header.vue";
import FeaturedProducts from "../components/FeaturedProducts.vue";
import Collections from "../components/Collections.vue";
import BestSeller from "../components/BestSeller.vue";
import Offers from "../components/Offers.vue";
import NewArrivals from "../components/NewArrivals.vue";
import Quotes from "../components/Quotes.vue";
import Blog from "../components/Blog.vue";
import Shop from "../components/Shop.vue";
import Brands from "../components/Brands.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Wrapper",
  components: {
    Nav,
    Header,
    FeaturedProducts,
    Collections,
    BestSeller,
    Offers,
    NewArrivals,
    Quotes,
    Blog,
    Shop,
    Brands,
    Footer,
  },
  data() {
    return {
      products: {
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
      },
    };
  },
};
</script>


<style scoped lang="scss">
</style>
