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
      <div class="card_items">
        <a class="card_item" href="" v-for="card in 4" :key="card.id">
          <img style="width: 100%" src="@/assets/img/card1.png" alt="card" />
          <div class="card_info">
            <h3 class="card_title">Пила</h3>
            <div class="card_teg">
              <p>скидка</p>
              <p>хит</p>
              <p>рассрочка</p>
            </div>

            <div class="card_prices">
              <div>
                <h4>Роозичная цена</h4>
                <span>300 000 руб</span>
              </div>
              <div>
                <h4>Клубная цена</h4>
                <span>100 000 руб</span>
              </div>
            </div>
            <button class="button_basket">basket</button>
          </div></a
        >
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

.card_items {
  display: flex;
  gap: 24px;
  flex-wrap: wrap;
  justify-content: space-between;
}

.card_item {
  border: 16px solid transparent;
  padding: 0px;
  &_image {
    img {
      width: 100%;
    }
  }

  .card_info {
    .card_title {
      font-size: 20px;
      margin-bottom: 12px;
    }
    .card_teg {
      display: flex;
      align-items: flex-start;
      flex-wrap: wrap;
      height: 100%;
      gap: 8px;
    }
    p {
      width: 40%;

      margin: 4px;
    }
    .card_prices {
      display: flex;
      justify-content: space-between;
      margin-top: 40px;
      gap: 40px;
      h4 {
        font-size: 14px;
        margin: 0px 0px 4px 0px;
      }
      span {
        font-size: 26px;
      }
    }
    .button_basket {
      margin-top: 16px;
      background: #ffee00;
      width: 100%;
      height: 48px;
      border: none;
      border-radius: 4px;
      padding: 12px 48px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
    }
  }
}

.menu {
  background: #ffffff;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;

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
