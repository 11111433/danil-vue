<script setup>
import Logo from "./Logo.vue";
</script>

<template>
  <section>
    <div class="section_content">
      <div class="menu mobile">
        <a href="">
          <img style="width: 100%" src="@/assets/img/home.svg" alt="home"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/home.svg" alt="home"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/home.svg" alt="home"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/home.svg" alt="home"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/home.svg" alt="home"
        /></a>
      </div>
      <h1 class="desktop">Season product</h1>
      <div class="section_group">
        <a href="">
          <span>Saw</span>
        </a>
        <a href="">
          <span>vacuum cleaner</span>
        </a>
        <a href="">
          <span>motoblock</span>
        </a>
        <a href="">
          <span>some thing</span>
        </a>
      </div>
      <div class="card">
        <a href="">
          <img style="width: 100%" src="@/assets/img/card1.png" alt="card"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/card1.png" alt="card"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/card1.png" alt="card"
        /></a>
        <a href="">
          <img style="width: 100%" src="@/assets/img/card1.png" alt="card"
        /></a>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
// :root {
//   --mobile: 1000px;
// }

$width: 1000px;
section {
  background: #f4f5f5;

  @media screen and (max-width: $width) {
    background: transparent;
  }
}
.section_content {
  max-width: calc(1920px - 192px - 192px);
  background: #f2f2f2;
  margin: 0 auto;

  height: auto;
  padding: 36px 8px;
}

.section_group {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  height: 100%;
  border: 16px solid transparent;
  gap: 16px;
}
a {
  color: #000000;
  background: #ffffff;
  text-decoration: none;

  border-radius: 20px;
  padding: 8px 12px;
  @media screen and (max-width: $width) {
    color: black;
  }
}
.card {
  background: #f4f5f5;
  display: flex;
  flex-wrap: nowrap;
  overflow-x: auto;

  border: 16px solid transparent;
  gap: 4px 30px;
  @media screen and (max-width: $width) {
    width: 1920px;
    height: auto;
  }
}

.menu {
  background: #ffffff;

  display: flex;
  justify-content: space-evenly;
}
.mobile {
  display: none;

  @media screen and (max-width: $width) {
    display: flex;
  }
}

.desktop {
  @media screen and (max-width: $width) {
    display: none;
  }
}
</style>
