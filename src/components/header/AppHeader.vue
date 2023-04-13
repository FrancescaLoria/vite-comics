<script>
export default {
  nome: "AppHeader",
  data() {
    const links = [
      {
        name: "Charachters",
        url: "#",
      },
      {
        name: "Comics",
        url: "#",
      },
      {
        name: "Movies",
        url: "#",
      },
      {
        name: "Tv",
        url: "#",
      },
      {
        name: "Games",
        url: "#",
      },
      {
        name: "Collectibles",
        url: "#",
      },
      {
        name: "Videos",
        url: "#",
      },
      {
        name: "Fans",
        url: "#",
      },
      {
        name: "News",
        url: "#",
      },
      {
        name: "Shop",
        url: "#",
      },
    ];
    return {
      links,
    };
  },
};
</script>

<template>
  <header>
    <div class="container">
      <img src="../../assets/img/dc-logo.png" alt="" />
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url">{{ link.name }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style scoped lang="scss">
header {
  height: 100px;
  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  img {
    width: 60px;
    object-fit: cover;
  }

  ul {
    display: flex;
    gap: 10px;
    font-size: 13px;
    font-weight: 600;
    li > a {
      text-transform: uppercase;
    }
  }
}
</style>
