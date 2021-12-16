<template>
  <footer>
    <section class="newsletter">
      <span><i class="far fa-envelope"></i></span>
    </section>
    <section class="about">
      <div class="container">
        <div class="column">
          <div class="logo">
            <img src="../assets/img/classic_shop_logo_footer.png" alt="logo" />
          </div>
          <div class="address">
            <p>12345 North Main Street,</p>
            <p>New York, NY 555555</p>
            <p>Phone: 1.800.555.12345</p>
            <p>Email: info@amalia.com</p>
            <p>Web: Theme-fusion</p>
          </div>

          <div class="social">
            <div class="icon"><i class="fab fa-facebook-f"></i></div>
            <div class="icon"><i class="fab fa-twitter"></i></div>
            <div class="icon"><i class="fab fa-instagram"></i></div>
            <div class="icon"><i class="fab fa-youtube"></i></div>
          </div>
        </div>
        <div class="column">
          <h4 class="title">TOP RATED PRODUCTS</h4>
          <ShopCard
            v-for="(item, i) in products"
            :key="`topRated-${i}`"
            :productName="item.product"
            :img="item.img"
            :price="item.price"
            :stars="item.stars"
            :by="item.by"
            :discount="item.discount"
            customClass="footer"
          />
        </div>
        <div class="column">
          <h4 class="title">RECENT POSTS</h4>
          <RecentPosts :recentPosts="recentPosts" />
        </div>
        <div class="column">
          <h4 class="title">TAGS</h4>
          <Tags :tags="tags" />
        </div>
      </div>
    </section>
    <section class="copyright"></section>
  </footer>
</template>

<script>
import ShopCard from "./ShopCard.vue";
import RecentPosts from "./RecentPosts.vue";
import Tags from "./Tags.vue";

export default {
  name: "Footer",
  components: {
    ShopCard,
    RecentPosts,
    Tags,
  },
  props: {
    products: Array,
  },
  data() {
    return {
      recentPosts: [
        {
          title:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry.",
          url: "https://wwww.google.com",
        },
        {
          title:
            "content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more.",
          url: "https://wwww.google.com",
        },
        {
          title:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry.",
          url: "https://wwww.google.com",
        },
        {
          title:
            "randomised words which don't look even slightly believable. If you are going.",
          url: "https://wwww.google.com",
        },
        {
          title:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry.",
          url: "https://wwww.google.com",
        },
      ],
      tags: [
        {
          name: "black",
          url: "https://wwww.google.com"
        },
        {
          name: "boots",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Brown",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Travel",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Warm",
          url: "https://wwww.google.com"
        }, 
        {
          name: "White",
          url: "https://wwww.google.com"
        }, 
        {
          name: "hat",
          url: "https://wwww.google.com"
        }, 
        {
          name: "summer",
          url: "https://wwww.google.com"
        }, 
        {
          name: "fabric",
          url: "https://wwww.google.com"
        }, 
        {
          name: "red",
          url: "https://wwww.google.com"
        }, 
        {
          name: "responsive",
          url: "https://wwww.google.com"
        }, 
        {
          name: "boots",
          url: "https://wwww.google.com"
        }, 
        {
          name: "winter",
          url: "https://wwww.google.com"
        }, 
        {
          name: "boots",
          url: "https://wwww.google.com"
        }, 
        {
          name: "honey",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Grey",
          url: "https://wwww.google.com"
        }, 
          {
          name: "boots",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Brown",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Travel",
          url: "https://wwww.google.com"
        }, 
        {
          name: "Warm",
          url: "https://wwww.google.com"
        }, 
        {
          name: "White",
          url: "https://wwww.google.com"
        }, 
        {
          name: "hat",
          url: "https://wwww.google.com"
        }, 
        {
          name: "summer",
          url: "https://wwww.google.com"
        }, 
        {
          name: "fabric",
          url: "https://wwww.google.com"
        }, 
        {
          name: "red",
          url: "https://wwww.google.com"
        }, 
        {
          name: "responsive",
          url: "https://wwww.google.com"
        }, 

      ],
    };
  },
};

</script>


<style scoped lang="scss">
footer {
  color: white;

  .container {
    display: flex;
    max-width: 1100px;
    margin: auto;
  }

  .newsletter {
    height: 200px;
    background-color: #303337;
  }

  .about {
    padding-top: 60px;
    padding-bottom: 60px;
    background-color: #2b2e32;
    .logo {
      img {
        max-width: 100%;
        width: 150px;
        margin-bottom: 40px;
      }
    }
    .address {
      margin-bottom: 40px;

      p {
        margin-bottom: 10px;
      }
    }

    .column {
      width: calc(25% - 20px);
      margin-right: 20px;

      .title {
        margin-bottom: 30px;
        font-size: 0.8em;
      }
    }
    .social {
      display: flex;
      align-items: center;
      .icon {
        margin: 0 6px;
        color: white;
      }
    }
  }

  .copyright {
    height: 100px;
    background-color: #1d1f22;
  }
}
</style>