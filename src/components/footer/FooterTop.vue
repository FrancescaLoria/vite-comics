<script>
export default {
  name: "FooterTop",
  data() {
    const links_1 = [
      {
        name: "DC COMICS",
        link: "#",
      },
      {
        name: "Charachters",
        link: "#",
      },
      {
        name: "Comics",
        link: "#",
      },
      {
        name: "Movies",
        link: "#",
      },
      {
        name: "Tv",
        link: "#",
      },
      {
        name: "Games",
        link: "#",
      },
      {
        name: "Videos",
        link: "#",
      },
      {
        name: "News",
        link: "#",
      },
    ];
    const links_2 = [
      {
        name: "SHOP",
        link: "#",
      },
      {
        name: "Shop DC",
        link: "#",
      },
      {
        name: "Shop DC Collectibles",
        link: "#",
      },
    ];
    const links_3 = [
      {
        name: "DC",
        link: "#",
      },
      {
        name: "Terms Of Use",
        link: "#",
      },
      {
        name: "Privacy policy (New)",
        link: "#",
      },
      {
        name: "Ad Choices",
        link: "#",
      },
      {
        name: "Adversting",
        link: "#",
      },
      {
        name: "Jobs",
        link: "#",
      },
      {
        name: "Subscriptions",
        link: "#",
      },
      {
        name: "Talent Workshop",
        link: "#",
      },
      {
        name: "CPSC Certificates",
        link: "#",
      },
      {
        name: "Ratings",
        link: "#",
      },
      {
        name: "Shop Help",
        link: "#",
      },
      {
        name: "Contact Us",
        link: "#",
      },
    ];
    const links_4 = [
      {
        name: "SITES",
        link: "#",
      },
      {
        name: "DC",
        link: "#",
      },
      {
        name: "MAD Magazine",
        link: "#",
      },
      {
        name: "DC Kids",
        link: "#",
      },
      {
        name: "DC Universe",
        link: "#",
      },
      {
        name: "DC Power Visa",
        link: "#",
      },
    ];
    return {
      links_1,
      links_2,
      links_3,
      links_4,
    };
  },
};
</script>

<template>
  <div class="footer-top">
    <div class="container">
      <div class="links">
        <div class="first-columns">
          <ul>
            <li v-for="(link, index) in links_1" :key="index">
              <span v-if="index === 0">{{ link.name }}</span>
              <a v-else :href="link.link">{{ link.name }}</a>
            </li>
          </ul>
          <ul>
            <li v-for="(link, index) in links_2" :key="index">
              <span v-if="index === 0">{{ link.name }}</span>
              <a v-else :href="link.link">{{ link.name }}</a>
            </li>
          </ul>
        </div>
        <div class="second-column">
          <ul>
            <li v-for="(link, index) in links_3" :key="index">
              <span v-if="index === 0">{{ link.name }}</span>
              <a v-else :href="link.link">{{ link.name }}</a>
            </li>
          </ul>
        </div>
        <div class="third-column">
          <ul>
            <li v-for="(link, index) in links_4" :key="index">
              <span v-if="index === 0">{{ link.name }}</span>
              <a v-else :href="link.link">{{ link.name }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="logo">
        <img src="../../assets/img/dc-logo-bg.png" alt="dc-logo" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-top {
  height: 320px;
  background-image: url("../../assets/img/footer-bg.jpg");
  background-size: 105%;
  .container {
    display: flex;
    justify-content: space-between;
    height: 100%;
    & > * {
      width: 50%;
    }

    .links {
      display: flex;
      gap: 50px;
      ul {
        padding-top: 30px;
        & > li:first-child {
          font-size: 18px;
          font-weight: 600;
          color: white;
        }

        a {
          font-size: 12px;
          color: #959595;
        }
      }
    }

    .logo {
      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
  }
}
</style>
