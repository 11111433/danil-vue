<script setup>
import Logo from "./Logo.vue";
</script>

<template>
  <header>
    <div class="header__content">
      <Logo class="mobile" />
      <div class="header__links">
        <a href="">
          <img src="@/assets/img/location.svg" alt="Location" />
          <span>Krsk</span>
        </a>
        <a href="" class="desktop">Shop</a>
        <a href="" class="desktop"
          ><span>Customers</span
          ><img src="@/assets/img/Vector.svg" alt="Arrow" />
        </a>
        <a href="" class="desktop"
          ><span>Company</span><img src="@/assets/img/Vector.svg" alt="Arrow"
        /></a>
        <a href="" class="desktop"
          ><span>Organization</span>
          <img src="@/assets/img/Vector.svg" alt="Arrow" />
        </a>
        <a href="" class="desktop">Sale</a>
        <a href="" class="desktop">Article</a>
        <a href="" class="desktop">Gift cards</a>
      </div>
      <div class="header_phone desktop">
        <a href="tel:+12312">12312</a>
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
// :root {
//   --mobile: 1000px;
// }

$width: 1000px;

header {
  background: #4d4d4d;

  @media screen and (max-width: $width) {
    background: transparent;
  }

  .header__content {
    max-width: calc(1920px - 192px - 192px);
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 44px;
    padding: 0 8px;
  }
}

a {
  color: #ffffff;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 4px;
  @media screen and (max-width: $width) {
    color: black;
  }
}

.header__links {
  display: flex;
  /* align-items: center; */
  gap: 24px;
}
.header_phone {
  display: flex;
}
/* .header__links a {
  margin-right: 24px;
}

.header__links a:last-child {
  margin-right: 0;
} */

.mobile {
  display: none;

  @media screen and (max-width: $width) {
    display: block;
  }
}

.desktop {
  @media screen and (max-width: $width) {
    display: none;
  }
}
</style>
