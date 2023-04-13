<script>
export default {
  name: "MainBottom",
};
</script>

<template>
  <div class="main-bottom">
    <div class="cont-info">
      <ul>
        <li>
          <img src="../../assets/img/buy-comics-digital-comics.png" alt="" />
          <a href="">DIGITAL COMICS</a>
        </li>
        <li>
          <img src="../../assets/img/buy-comics-digital-comics.png" alt="" />
          <a href="">DIGITAL COMICS</a>
        </li>
        <li>
          <img src="../../assets/img/buy-comics-digital-comics.png" alt="" />
          <a href="">DIGITAL COMICS</a>
        </li>
        <li>
          <img src="../../assets/img/buy-comics-digital-comics.png" alt="" />
          <a href="">DIGITAL COMICS</a>
        </li>
        <li>
          <img src="../../assets/img/buy-comics-digital-comics.png" alt="" />
          <a href="">DIGITAL COMICS</a>
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
      li {
        display: flex;
        align-items: center;
        gap: 10px;
        font-size: 12px;
        img {
          width: 35px;
          object-fit: cover;
        }
      }
    }
  }
}
</style>
