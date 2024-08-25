<script setup lang="ts">
import MusicCard from './MusicCard.vue';
</script>

<template>
<h2 class="w-[100%] text-[2rem] px-12 text-white">音乐</h2>

<div class="container w-[100%] flex flex-wrap justify-start p-[2rem]">
  <template v-for="_ in 8"> 
    <MusicCard title="blade"/>
  </template>
</div>
</template>

<style scoped>

</style>