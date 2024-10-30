<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'
</script>

<template>
  <!-- <Drawer> </Drawer> -->
  <div class="screen">
    <Header />
    <div class="spacing">
      <div class="mainBlock">
        <h2 class="mainText">Все кроссовки</h2>
        <div class="searchAndSortBlock">
          <select class="selectorSortSneackers">
            <option>По названию</option>
            <option>По цене (сначала дешевле)</option>

            <option>По цене (сначала дороже)</option>
          </select>

          <div class="searchBlock">
            <img class="searchImage" src="/search.svg" alt="" />
            <input class="searchInput" type="text" placeholder="Поиск..." />
          </div>
        </div>
      </div>
      <!-- <CardList /> -->
    </div>
  </div>
</template>
<style scoped>
.screen {
  background-color: white;
  width: 80%;
  margin: auto;
  border-radius: 0.75rem;
  box-shadow:
    0 20px 25px -5px rgb(0 0 0 / 0.1),
    0 8px 10px -6px rgb(0 0 0 / 0.1);
  margin-top: 3.5rem;
}

.spacing {
  padding: 2.5rem;
}

.mainBlock {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.mainText {
  font-size: 1.875rem;
  line-height: 2.25rem;
  font-weight: 700;
  margin-bottom: 2rem;
}
.searchAndSortBlock {
  display: flex;
  gap: 1rem;
}
.selectorSortSneackers {
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  padding-left: 0.75rem;
  padding-right: 0.75rem;
  border: solid;
  border-width: 1px;
  border-radius: 0.375rem;
  outline: 2px solid transparent;
  outline-offset: 2px;
  border-color: rgb(209 213 219);
}
.searchBlock {
  position: relative;
}
.searchImage {
  position: absolute;
  left: 16px;
  top: 12px;
}
.searchInput {
  border: solid;
  border-radius: 0.375rem;
  border-width: 1px;
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  padding-left: 2.75rem;
  padding-right: 1rem;
  outline: 2px solid transparent;
  outline-offset: 2px;
  border-color: rgb(209 213 219);
}
.searchInput:focus {
  border-color: rgb(156 163 175);
}
</style>
