<script setup></script>

<template>
  <header>
    <div class="header__content">
      <div class="header__links">
        <a href="">
          <img src="@/assets/img/location.svg" alt="Location" />
          <span>Krsk</span>
        </a>
        <a href="">Shop</a>
        <a href=""
          ><span>Customers</span
          ><img src="@/assets/img/Vector.svg" alt="Arrow" />
        </a>
        <a href=""
          ><span>Company</span><img src="@/assets/img/Vector.svg" alt="Arrow"
        /></a>
        <a href=""
          ><span>Organization</span>
          <img src="@/assets/img/Vector.svg" alt="Arrow" />
        </a>
        <a href="">Sale</a>
        <a href="">Article</a>
        <a href="">Gift cards</a>
      </div>
      <div class="header_phone">
        <a href="tel:+12312">12312</a>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  background: #4d4d4d;
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

a {
  color: #ffffff;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 4px;
}

.header__links {
  display: flex;
  /* align-items: center; */
  gap: 24px;
}
.header_phone {
  display: flex;

  margin-right: 193px;
}
/* .header__links a {
  margin-right: 24px;
}

.header__links a:last-child {
  margin-right: 0;
} */
</style>
