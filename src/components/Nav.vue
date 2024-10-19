<script setup>
import Logo from "./Logo.vue";
</script>

<template>
  <nav>
    <div class="nav_content">
      <div style="display: flex; align-items: center; gap: 12px">
        <Logo class="desktop" />
        <button class="button_catalog mobile">
          <span />
          Catalog
        </button>

        <!-- <div class="nav_catalog">
          <div class="nav_burger">
            <a href="">
              <img src="@/assets/img/Rectangleup.svg" alt="up" /><img
                src="@/assets/img/Rectangledown.svg"
                alt="down"
            /></a>
          </div>
          <div class="catalog">
            <a href=""><span class="text_catalog">КАТАЛОГ</span></a>
          </div>
        </div> -->
      </div>

      <div class="nav_menu desktop">
        <a href="">
          <img src="@/assets/img/clock.svg" alt="clock" />
          <span>status</span>
        </a>
        <a href="">
          <img src="@/assets/img/Iconstat.svg" alt="Iconstat" />
          <span>comparison</span>
        </a>
        <a href="">
          <img src="@/assets/img/icon_favorite.svg" alt="favorite" />
          <span>favourites</span>
        </a>
        <a href="">
          <img src="@/assets/img/Frame.svg" alt="frame" />
          <span>34 000</span>
        </a>
        <a href="">
          <img src="@/assets/img/person.svg" alt="person" />
          <span>login/registration</span>
        </a>
      </div>
    </div>
  </nav>
</template>

<style scoped lang="scss">
$width: 1000px;
nav {
  background: #ffffff;
}
.nav_content {
  max-width: calc(1920px - 195px - 195px);
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-flow: row nowrap;
  height: 59px;
  padding: 0 8px;
}

.nav_catalog {
  max-width: calc(135px - 40px);
  background: var(--yellow);
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin: 10px 165px 10px 19px;
  // margin-top: 10px;
  // margin-right: 165px;
  // margin-bottom: 10px;
  // margin-left: 19px;
  height: 100%;
  width: 100%;
  gap: 4px 24px;
}

.button_catalog {
  background: var(--yellow);
  border: none;
  border-radius: 4px;
  padding: 8px 22px;
  display: flex;
  align-items: center;
  gap: 2px;

  span {
    position: relative;
    display: block;
    height: 24px;
    width: 24px;

    &::after,
    &::before {
      position: absolute;
      content: "";
      width: 100%;
      height: 2px;
      background: black;
      left: 0;
    }

    &::before {
      top: 8px;
    }

    &::after {
      bottom: 8px;
      width: 70%;
    }
  }
}

.nav_burger {
  display: flex;

  margin: auto;
  gap: 1px;
  height: 100%;
  width: 10%;
}

.text_catalog {
  color: #000000;
  font-weight: 400;
  font-family: "Rubik";
  font-size: 14px;
  line-height: 16px;
}

.nav_menu {
  display: flex;
  align-items: center;
  gap: 24px;
}
a {
  color: #000000;
  text-decoration: none;
  display: flex;
  align-items: center;
  flex-flow: row nowrap;
  height: 100%;
  gap: 0px;
}
.desktop {
  @media screen and (max-width: $width) {
    display: none;
  }
}

.mobile {
  @media screen and (max-width: $width) {
    display: block;
  }
}
</style>
