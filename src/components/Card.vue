<script setup>
defineProps({
  title: String,
  imageUrl: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickFav: Function
})
</script>

<template>
  <div class="card">
    <!-- <img src="/like-1.svg" alt="Like 1" class="absolute top-8 left-8" /> -->
    <img
      @click="onClickFav"
      :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
      alt="Like"
      class="absolute top-8 left-8"
    />
    <img :src="imageUrl" alt="Sneaker" />
    <p class="mt-2">{{ title }}</p>
    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена</span>
        <b>{{ price }}</b>
      </div>
      <img @click="onClickAdd" :src="isAdded ? '/checked.svg' : '/plus.svg'" alt="Plus" />
    </div>
  </div>
</template>
<style scoped>
.card {
  position: relative;
  background-color: white;
  border-width: 1px;
  border-color: rgb(241, 245, 249);
  border-radius: 1.5rem;
  padding: 2rem;
  cursor: pointer;
}
.card:hover {
  transform: translateY(-0.5rem);
  box-shadow:
    0 20px 25px -5px rgb(0 0 0 / 0.1),
    0 8px 10px -6px rgb(0 0 0 / 0.1);
}
</style>
