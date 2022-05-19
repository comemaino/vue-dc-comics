<template>
  <footer id="footer">
    <section id="top">
      <div class="container">
        <div class="col left">
          <div class="links-col">
            <h3>dc comics</h3>
            <ul>
              <li
                v-for="(item, index) in dcComicsLinks"
                :key="index"
                :class="{ active: item.active }"
              >
                <a href="">{{ item.text }} </a>
              </li>
            </ul>

            <h3>shop</h3>
            <ul>
              <li
                v-for="(item, index) in shopLinks"
                :key="index"
                :class="{ active: item.active }"
              >
                <a href="">{{ item.text }} </a>
              </li>
            </ul>
          </div>
          <div class="links-col">
            <h3>dc</h3>
            <ul>
              <li
                v-for="(item, index) in dcLinks"
                :key="index"
                :class="{ active: item.active }"
              >
                <a href="">{{ item.text }} </a>
              </li>
            </ul>
          </div>
          <div class="links-col">
            <h3>sites</h3>
            <ul>
              <li
                v-for="(item, index) in sitesLinks"
                :key="index"
                :class="{ active: item.active }"
              >
                <a href="">{{ item.text }} </a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col right">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </section>
    <section id="bottom"></section>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  data: function () {
    return {
      dcComicsLinks: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: false,
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
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
      ],

      shopLinks: [
        {
          url: "#",
          text: "Shop DC",
          active: false,
        },
        {
          url: "#",
          text: "Shop DC Collectibles",
          active: false,
        },
      ],

      dcLinks: [
        {
          url: "#",
          text: "Terms Of Use",
          active: false,
        },
        {
          url: "#",
          text: "Privacy Policy (New)",
          active: false,
        },
        {
          url: "#",
          text: "Ad Chioces",
          active: false,
        },
        {
          url: "#",
          text: "Advertising",
          active: false,
        },
        {
          url: "#",
          text: "Jobs",
          active: false,
        },
        {
          url: "#",
          text: "Subsciption",
          active: false,
        },
        {
          url: "#",
          text: "Talent Workshops",
          active: false,
        },
        {
          url: "#",
          text: "CPSC Certificates",
          active: false,
        },
        {
          url: "#",
          text: "Ratings",
          active: false,
        },
        {
          url: "#",
          text: "Shop Help",
          active: false,
        },
        {
          url: "#",
          text: "Contact Us",
          active: false,
        },
      ],

      sitesLinks: [
        {
          url: "#",
          text: "DC",
          active: false,
        },
        {
          url: "#",
          text: "MAD Magazine",
          active: false,
        },
        {
          url: "#",
          text: "DC Kids",
          active: false,
        },
        {
          url: "#",
          text: "DC Universe",
          active: false,
        },
        {
          url: "#",
          text: "DC Power Visa",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../components/style/common.scss";

#footer {
  height: 400px;

  #top {
    padding: 2rem 0;
    height: 350px;
    background-image: url(../assets/img/footer-bg.jpg);

    overflow: hidden;

    .col {
      display: flex;
      justify-content: flex-start;

      &.right {
        align-items: center;
      }

      img {
        height: 140%;
      }

      .links-col {
        margin: 0.5rem 1rem;
        display: flex;
        flex-direction: column;

        ul {
          margin: 0.5rem 0 1rem;

          li {
            line-height: 1.3rem;
          }
        }

        h3 {
          text-transform: uppercase;
          color: #fff;
        }

        a {
          color: #888;
        }
      }
    }
  }

  #bottom {
    height: 80px;
    background-color: #555;
  }
}
</style>
