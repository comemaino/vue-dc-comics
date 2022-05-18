<template>
  <section id="shop-section">
    <div class="container">
      <ul class="buy-links">
        <li v-for="(item, index) in links" :key="index">
          <img :src="require(`../assets/img/${item.img}`)" alt="" />
          <a href="">
            <h4>{{ item.text }}</h4>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppShopSection",

  data: function () {
    return {
      links: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "DC Merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "Comics Shop Locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../components/style/common.scss";

#shop-section {
  height: 100px;
  line-height: 100px;
  color: #fff;
  background-color: #29f;

  .buy-links {
    display: flex;
    justify-content: space-between;

    li {
      display: flex;
      align-items: center;

      img {
        margin: 1rem;
        height: 50%;
      }

      a {
        color: #fff;
        text-transform: uppercase;

        h4 {
          font-size: 1rem;
        }
      }
    }
  }
}
</style>
