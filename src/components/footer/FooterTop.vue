<script>
export default {
  name: "FooterTop",
  data() {
    const links = [
      [
        [
          {
            name: "dc comics",
            link: "#",
          },
          {
            name: "charachters",
            link: "#",
          },
          {
            name: "comics",
            link: "#",
          },
          {
            name: "movies",
            link: "#",
          },
          {
            name: "tv",
            link: "#",
          },
          {
            name: "games",
            link: "#",
          },
          {
            name: "videos",
            link: "#",
          },
          {
            name: "news",
            link: "#",
          },
        ],
        [],
      ],
      [[]],
      [[]],
    ];
    return {
      links,
    };
  },
};
</script>

<template>
  <div class="footer-top">
    <div class="container">
      <div class="links">
        <div v-for="(row, index1) in links" :key="index1">
          <ul v-for="(list, index2) in row" :key="index2">
            <li v-for="(finalLinks, index3) in list" :key="index3">
              <a :href="finalLinks.url">{{ finalLinks.name }}</a>
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
          text-transform: uppercase;
        }

        a {
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
