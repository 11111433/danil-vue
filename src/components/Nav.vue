<script setup></script>

<template>
  <nav>
    <div class="nav_content">
      <div class="nav_salelom">
        <img src="@/assets/img/salelom.svg" alt="salelom" />
      </div>

      <div class="nav_catalog">
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
      </div>
      <div class="nav_menu">
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

<style scoped>
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
.nav_salelom {
  width: 109px;
  height: 32px;
  display: flex;
  gap: 10px;
}
.nav_catalog {
  max-width: calc(135px - 40px);
  background: #ffee00;
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-top: 10px;
  margin-right: 165px;
  margin-bottom: 10px;
  height: 100%;
  margin-left: 19px;
  width: 100%;
  gap: 4px 24px;
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
</style>
