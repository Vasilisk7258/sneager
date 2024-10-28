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
