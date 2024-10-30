<template>
  <header class="header">
    <div class="logo_box">
      <img src="/logo.png" alt="Logo" class="logo-image" />
      <div>
        <h2 class="main-text">KIRILKA Sneakers</h2>
        <p class="text-best-shop">Лучший магазин</p>
      </div>
    </div>
    <ul class="ul">
      <li class="li">
        <img src="/cart.svg" alt="Cart" />
        <b>1205 руб.</b>
      </li>
      <li class="li">
        <img src="/heart.svg" alt="Cart" />
        <span>Закладки</span>
      </li>
      <li class="li">
        <img src="/profile.svg" alt="Cart" />
        <span>Профиль</span>
      </li>
    </ul>
  </header>
</template>
<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  border-color: rgb(226 232 240);
  border-bottom-width: 1px;
  padding-left: 2.5rem;
  padding-right: 2.5rem;
  padding-top: 2rem;
  padding-bottom: 2rem;
}
.logo_box {
  display: flex;
  justify-items: center;
  gap: 1rem;
}
.logo-image {
  width: 90px;
}
.main-text {
  font-weight: 600;
  font-size: 1.4rem;
  line-height: 1.75rem;
  text-transform: uppercase;
}
.text-best-shop {
  color: rgb(148 163 184);
}
.ul {
  /* display: flex; */
  justify-items: center;
  gap: 2.5rem;
}
.li {
  display: flex;
  justify-items: center;
  gap: 1rem;
  cursor: pointer;
  color: rgb(148 163 184);
  padding-bottom: 5px;
}
.li:hover {
  color: black;
}
</style>
