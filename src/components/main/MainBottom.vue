<script>
export default {
  name: "MainBottom",
  data() {
    const links = [
      {
        img: "buy-comics-digital-comics.png",
        url: "#",
        text: "Digital comics",
      },
      {
        img: "buy-comics-merchandise.png",
        url: "#",
        text: "dc merchandise",
      },
      {
        img: "buy-comics-subscriptions.png",
        url: "#",
        text: "Subscription",
      },
      {
        img: "buy-comics-shop-locator.png",
        url: "#",
        text: "Comic shop locator",
        resize: true,
      },
      {
        img: "buy-dc-power-visa.svg",
        url: "#",
        text: "DC power visa",
      },
    ];
    return {
      links,
    };
  },
  methods: {
    getImageUrl(img) {
      return new URL(`../../assets/img/${img}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="main-bottom">
    <div class="cont-info">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <img
            :src="getImageUrl(link.img)"
            :alt="link.url"
            :class="link.resize ? 'resize' : ''"
          />
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
.main-bottom {
  height: 150px;
  background-color: #0282f9;
  color: white;
  display: flex;
  align-items: center;

  .cont-info {
    width: 60%;
    margin: 0 auto;

    ul {
      display: flex;
      justify-content: space-between;
      text-transform: uppercase;
      li {
        display: flex;
        align-items: center;
        gap: 10px;
        font-size: 12px;
        img {
          width: 35px;
          object-fit: cover;
          &.resize {
            transform: scale(0.8);
          }
        }
      }
    }
  }
}
</style>
