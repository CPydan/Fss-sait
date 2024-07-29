<script setup>
defineProps({
  imageUrl: String,
  title: String,
  description: String,
  textLink: String
})

const myLink = () => {
  alert('Нажми меня')
}
</script>

<template>
  <div class="flex flex-col items-center text-center w-72 mx-auto">
    <img class="m-70 h-70" :src="imageUrl" alt="Info image" />
    <h2 class="mt-4 text-2xl font-medium">{{ title }}</h2>
    <p class="text-gray-400 mt-2">{{ description }}</p>
    <a href="https://t.me/d1n_yaa" @onclick="myLink">{{ textLink }}</a>
  </div>
</template>
