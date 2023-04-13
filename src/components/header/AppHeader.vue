<script>
export default {
  nome: "AppHeader",
};
</script>

<template>
  <header>
    <div class="container">
      <img src="../../assets/img/dc-logo.png" alt="" />
      <ul>
        <li>characters</li>
        <li>characters</li>
        <li>characters</li>
        <li>characters</li>
        <li>characters</li>
        <li>characters</li>
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
  }
}
</style>
