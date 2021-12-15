<template>
  <nav>
    <div class="upper-nav">
      <div class="container">
        <div class="social">
          <div class="icon"><i class="fab fa-facebook-f"></i></div>
          <div class="icon"><i class="fab fa-twitter"></i></div>
          <div class="icon"><i class="fab fa-instagram"></i></div>
          <div class="icon"><i class="fab fa-youtube"></i></div>
        </div>
        <div class="account">
          <div>
            <span>Shopping Cart</span>
          </div>
          <div class="my-account">
            <span>My Account</span>
            <span class="arrow"><i class="fas fa-chevron-down"></i></span>
          </div>
          <div class="cart">
            <span class="cart-icon"><i class="fas fa-shopping-cart"></i></span>
            <span>CART</span>
            <span class="arrow"><i class="fas fa-chevron-down"></i></span>
          </div>
        </div>
      </div>
    </div>
    <div class="bottom-nav">
      <div class="container">
        <div class="logo">
          <img src="../../assets/img/classic_shop_logo1x.png" alt="" />
        </div>
        <div class="menu">
          <ul>
            <NavItem
              v-for="(item, i) in navigation"
              :key="{ i }"
              :label="item.label"
              :children="item.children"
            />
          </ul>
          <div class="button">
            <Button :text="buttonText" :blue="style" />
          </div>
          <div class="search"><i class="fas fa-search"></i></div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import NavItem from "./NavItem.vue";
import Button from "../Button.vue";
export default {
  name: "Nav",
  components: {
    NavItem,
    Button,
  },
  data: function () {
    return {
      buttonText: "SHOP NOW!",
      style: true,
      navigation: [
        {
          label: "Home",
          children: [
            {
              label: "Shop",
            },
            {
              label: "Account",
            },
          ],
        },
        {
          label: "Shop",
          children: [
            {
              label: "Men",
            },
            {
              label: "Women",
            },
          ],
        },
        {
          label: "Products",
          children: [
            {
              label: "Clothes",
            },
            {
              label: "Accesories",
            },
          ],
        },
        {
          label: "Categories",
          children: [
            {
              label: "T-shirts",
            },
            {
              label: "Pants",
            },
            {
              label: "Shoes",
            },
          ],
        },
        {
          label: "News",
        },
        {
          label: "Elements",
          children: [
            {
              label: "Featured Products",
            },
            {
              label: "Best Seller",
            },
            {
              label: "New Arrivals",
            },
            {
              label: "Blog",
            },
          ],
        },
      ],
    };
  },
};
</script>


<style scoped lang="scss">
nav {
  margin: auto;
  background: white;
  min-width: 1200px;
  .upper-nav {
    border-bottom: 1px solid #ebebeb;
  }
  .bottom-nav {
    display: flex;
    justify-content: space-between;
    .container {
      height: 80px;
      .menu {
        display: flex;
        align-items: center;
      }
      .logo {
        display: flex;
        align-items: center;
      }
    }
  }
  .container {
    width: 70%;
    margin: auto;
    display: flex;
    height: 40px;
    justify-content: space-between;
  }
  .social {
    display: flex;
    align-items: center;
    .icon {
      margin: 0 6px;
      color: rgb(88, 87, 87);
    }
  }
  .account {
    display: flex;
    align-items: center;
    font-size: 0.7em;
    font-weight: 700;
    color: #585758;
    .my-account {
      border-right: 1px solid #ebebeb;
      border-left: 1px solid #ebebeb;
    }
    .arrow {
      margin: 0 5px;
    }

    div {
      height: 100%;
      line-height: 40px;
      padding: 0 6px;
      &.cart {
        background-color: #f9f9f9;
        width: 120px;
        text-align: center;
      }
      span {
        display: inline-block;
        vertical-align: middle;
        height: 100%;
        line-height: 40px;
        &.cart-icon {
          margin: 0 5px;
        }
      }

      .arrow {
        font-size: 12px;
        font-weight: 200;
      }
    }
  }
}
</style>