<script setup lang="ts">
defineProps({
  title: {
    type: String,
    defualt: 'Blade'
  }
})
</script>

<template>
  <div class="card flex flex-col w-[16rem] h-[20rem] m-[1rem] bg-black justify-between
    hover:translate-y-[-10px] transition-transform duration-300">
    <main class="flex flex-col justify-center p-[1rem]">
      <h2 class=" text-white">{{ title }}</h2>
      kaokao
    </main>
    <figure class="">
    <img
      src="/src/assets/uploads/Kaokao_Blade.png"
      alt="trance"
    />
  </figure>
  </div>
</template>

<style scoped></style>