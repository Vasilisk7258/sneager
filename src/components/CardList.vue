<script setup>
import Card from './Card.vue'
const onClickAdd = () => {
  alert(111)
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      title="Мужские кроссовки Nike Blazer Mid Suede"
      image-url="/sneakers/sneakers-1.jpg"
      :price="5000"
      v-on:click-add="onClickAdd"
    />
    <!-- <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card /> -->
  </div>
</template>
