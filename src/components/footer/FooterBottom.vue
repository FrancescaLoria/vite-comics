<script>
export default {
  name: "FooterBottom",
};
</script>

<template>
  <div class="footer-bottom">
    <div class="container">
      <div class="button">
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="links">
        <ul>
          <li>FOLLOW US</li>
          <li>
            <img src="../../assets/img/footer-facebook.png" alt="facebook" />
          </li>
          <li>
            <img src="../../assets/img/footer-twitter.png" alt="twitter" />
          </li>
          <li>
            <img src="../../assets/img/footer-youtube.png" alt="youtube" />
          </li>
          <li>
            <img src="../../assets/img//footer-pinterest.png" alt="pinterest" />
          </li>
          <li>
            <img src="../../assets/img/footer-periscope.png" alt="periscope" />
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-bottom {
  background-color: #303030;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .button {
      border: 2px solid #0282f9;
      padding: 12px;
      margin: 20px 0;
      display: flex;
      align-items: center;
      justify-content: center;
      button {
        background-color: unset;
        border: none;
        color: white;
        font-weight: 600;
      }
    }

    .links {
      ul {
        display: flex;
        align-items: center;
        gap: 15px;

        & > li:first-child {
          color: #0282f9;
          font-weight: 600;
          font-size: 18px;
        }
      }
    }
  }
}
</style>
