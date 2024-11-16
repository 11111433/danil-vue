<template>
  <div class="card-item" href="#">
    <img src="@/assets/img/card1.png" alt="card" class="card-item__image" />

    <div class="card-item__icon">
      <img
        src="@/assets/img/favorite.svg"
        alt="favorite"
        class="card-item__icon-image card-item__icon-image--favorite"
      />
      <img
        src="@/assets/img/comparison.svg"
        alt="comparison"
        class="card-item__icon-image card-item__icon-image--comparison"
      />
    </div>
    <div class="card-item__info">
      <h3 class="card-item__title">
        <a href="">Пила</a>
      </h3>
      <div class="card-item__tags">
        <p class="card-item__tag">скидка</p>
        <p class="card-item__tag">хит</p>
        <p class="card-item__tag">рассрочка</p>
      </div>
      <div class="card-item__prices">
        <div class="card-item__price">
          <h4 class="card-item__price-title">Розничная цена</h4>
          <span class="card-item__price-value">300 000 руб</span>
        </div>
        <div class="card-item__price">
          <h4 class="card-item__price-title">Клубная цена</h4>
          <span class="card-item__price-value">100 000 руб</span>
        </div>
      </div>
      <button class="button button--basket">basket</button>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.card-item {
  position: relative;
  border: 16px solid transparent;
  background: white;
  border-radius: 12px;
  overflow: hidden; /* Added for visual effect when image overflows card borders */
  transition: box-shadow 0.3s; /* Added smooth effect on hover */
}

.card-item:hover {
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1); /* Hover effect */
}

.card-item__image {
  width: 100%;
}

.card-item__icon {
  position: absolute;
  right: 12px;
  top: 12px;
}

.card-item__icon-image {
  display: block;
}

.card-item__icon-image--favorite {
  top: 16px;
}

.card-item__icon-image--comparison {
  top: 40px;
}

.card-item__info {
  padding: 16px; /* Added internal padding for the card */
}

.card-item__title {
  font-size: 20px;
  margin-bottom: 12px;
}

.card-item__tags {
  display: flex;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 8px;
}

.card-item__tag {
  background: #f0f0f0; /* Background for tags */
  border-radius: 4px; /* Rounding for tag corners */
  padding: 4px 8px;
}

.card-item__prices {
  display: flex;
  justify-content: space-between;
  margin-top: 40px;
  gap: 40px;
}

.card-item__price {
}

.card-item__price-title {
  font-size: 14px;
  margin: 0px 0px 4px 0px;
}

.card-item__price-value {
  font-size: 26px;
  color: #e80000; /* Color for prices */
  font-weight: bold; /* Highlighting price */
}

.button--basket {
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
  transition: background 0.3s; /* Smooth background transition */
}

.button--basket:hover {
  background: #ffd700; /* button highlight on hover */
}
</style>
