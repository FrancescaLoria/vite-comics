<script>
export default {
  name: "FooterTop",
};
</script>

<template>
  <div class="footer-top">
    <div class="container">
      <div class="links">
        <div class="first-column">
          <ul>
            <li>Dc comics</li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
          </ul>

          <ul>
            <li>Dc comics</li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
          </ul>
        </div>

        <div class="second-column">
          <ul>
            <li>Dc comics</li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
          </ul>
        </div>

        <div class="third-column">
          <ul>
            <li>Dc comics</li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
            </li>
            <li>
              <a href="#">Charachters</a>
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
