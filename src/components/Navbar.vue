<template>
  <div class="menu menu--mobile">
    <a href="#" class="menu__item">
      <img src="@/assets/img/home.svg" alt="home" class="menu__icon" />
    </a>
    <a href="#" class="menu__item">
      <img src="@/assets/img/home.svg" alt="home" class="menu__icon" />
    </a>
    <a href="#" class="menu__item">
      <img src="@/assets/img/home.svg" alt="home" class="menu__icon" />
    </a>
    <a href="#" class="menu__item">
      <img src="@/assets/img/home.svg" alt="home" class="menu__icon" />
    </a>
    <a href="#" class="menu__item">
      <img src="@/assets/img/home.svg" alt="home" class="menu__icon" />
    </a>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.menu {
  background: #ffffff;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.1); /* Added shadow to highlight menu. */
}

.menu--mobile {
  display: none;
}

@media screen and (max-width: 1000px) {
  .menu--mobile {
    display: flex;
  }
}

.menu__item {
  color: #000000;
  text-decoration: none;
  padding: 10px; /* Added padding for clickability */
}

.menu__icon {
  width: 32px; /* Specified width for icons */
}
</style>
