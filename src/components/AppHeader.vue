<template>
  <header id="header">
    <div class="container">
      <div class="col">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <nav class="col">
        <ul class="header__menu">
          <li
            v-for="(item, index) in links"
            :key="index"
            :class="{ active: item.active }"
          >
            <a href="">{{ item.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      links: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "Tv",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Collectibles",
          active: true,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../components/style/common.scss";

#header {
  width: 100%;
  height: 100px;
  line-height: 100px;
  border: 1px solid #f00;

  .col {
    height: 100px;
    line-height: 100px;
    border: 1px solid #00f;

    li {
      display: inline-block;
      margin: 0 0.5rem;

      a {
        color: #444;
        text-transform: uppercase;
      }
    }
  }
}

img {
  width: 4rem;

  vertical-align: middle;
}
</style>
