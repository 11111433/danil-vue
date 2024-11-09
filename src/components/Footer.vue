<script setup>
import Logo from "./Logo.vue";
</script>

<template>
  <footer>
    <div class="footer_content">
      <div class="footer_menu desktop">
        <h1>Популярные категории</h1>
        <div>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>mobile and desktop</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>web</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>photo</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>auto</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>for home</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>for kitchen</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>buety</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>instruments</span>
          </a>
          <a href="">
            <img src="@/assets/img/mobile.svg" alt="mobile" />
            <span>sport</span>
          </a>
        </div>
        <div class="footer_delete">
          <a href="">
            <span>delete</span>
          </a>
        </div>
      </div>
      <div class="footer_slider mobile">
        <div>
          <a href="">
            <img
              style="width: 100%"
              src="@/assets/img/slider.svg"
              alt="slider"
            />
          </a>
        </div>
        <h1>SALE</h1>
        <div class="footer_sale">
          <a href="">
            <img
              style="width: 100%"
              src="@/assets/img/cardsalle.svg"
              alt="cardsalle"
            />
          </a>
          <a href="">
            <img
              style="width: 100%"
              src="@/assets/img/cardsalle.svg"
              alt="cardsalle"
            />
          </a>
          <a href="">
            <img
              style="width: 100%"
              src="@/assets/img/cardsalle.svg"
              alt="cardsalle"
            />
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
// :root {
//   --mobile: 1000px;
// }

$width: 1000px;

footer {
  background: #ffffff;

  @media screen and (max-width: $width) {
    background: transparent;
  }

  .footer_content {
    max-width: calc(1920px - 192px - 192px);
    margin: 0 auto;
    display: flex;
    justify-content: space-between;

    height: 100%;
    padding: 0 8px;
    gap: 30px;
  }
}

a {
  color: #000000;
  text-decoration: none;
  display: flex;
  align-items: center;
  height: 100%;
  // gap: 10px;
  margin: 12px 2px 2px 2px;
}
.footer_menu {
  // max-width: calc(360px - 730px);
  display: flex;
  flex-direction: column;
  align-items: stretch;
  margin: 2px 2px 16px 2px;
  height: 80%;
  width: 20%;
  border: #f2f2f2;
  // gap: 2px;
}
.footer_delete {
  // max-width: calc(360px - 80px);
  height: 100%;
  width: 100%;
  gap: 16px 24px;
  margin: 16px 2px 2px 2px;
}
.footer_slider {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  height: 100%;
  width: 80%;
}
.footer_sale {
  display: flex;
  // flex-direction: row;
  // justify-content: space-between;
  // height: 100%;
  // width: 100%;
  margin: 24px 0px;
  gap: 4px 30px;
}

.mobile {
  @media screen and (max-width: $width) {
    display: block;
    width: 100%;
  }
}

.desktop {
  @media screen and (max-width: $width) {
    display: none;
  }
}
</style>
