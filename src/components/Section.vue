<script setup>
import CardProduct from "./CardProduct.vue";
import Logo from "./Logo.vue";
</script>

<template>
  <section class="section">
    <div class="section__content">
      <h1 class="section__title section__title--desktop">Season product</h1>
      <div class="section__group">
        <a href="#" class="section__link">
          <span class="section__link-text">Saw</span>
        </a>
        <a href="#" class="section__link">
          <span class="section__link-text">vacuum cleaner</span>
        </a>
        <a href="#" class="section__link">
          <span class="section__link-text">motoblock</span>
        </a>
        <a href="#" class="section__link">
          <span class="section__link-text">some thing</span>
        </a>
      </div>
      <div class="card-items">
        <CardProduct v-for="card in 4" :key="card.id" />
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.section {
  background: #f4f5f5;
}

@media screen and (max-width: 1000px) {
  .section {
    background: transparent;
  }
}

.section__content {
  max-width: calc(1920px - 192px - 192px);
  background: #f2f2f2;
  margin: 0 auto;
  padding: 36px 8px;
  border-radius: 12px; /* Added corner rounding for better visual perception. */
}

.section__group {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  border: 16px solid transparent;
  gap: 16px;
}

.section__link {
  color: #000000;
  background: #ffffff;
  text-decoration: none;
  border-radius: 20px;
  padding: 8px 12px;
  transition: background 0.3s; /* Added transition for smooth background change */
}

.section__link:hover {
  background: #f0f0f0; /* Hover effect */
}

@media screen and (max-width: 1000px) {
  .section__link {
    color: black;
  }
}

.card-items {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 24px; /* Added gap between cards */
}
</style>
