<script lang="ts" setup>

const navItems = [
  { text: 'MUSIC' },
  { text: 'LABELS' },
  { text: 'RADIO' },
  { text: 'ARTISTS' },
  { text: 'ABOUT' }
]
</script>

<template>
  <div class="fixed z-10 top backdrop-blur flex justify-between w-50rem px-6 py-2 mb-5 rounded-[3rem] border border-white/20">
    <a class="flex items-center" href="/home">
      <img src="../../assets/img/logo.png" class="w-16" alt="Cooperation"/>
      <div class="absolute ml-3 w-9 h-9 bg-neutral-50 blur-lg"></div>
    </a>
    <ul class="flex items-center">
      <li v-for="item in navItems" :key="item.text">
        <a :href="item.text"
           class="text-gray-400 hover:text-white transition mx-8">
          {{ item.text }}
        </a>
      </li>
    </ul>
    <a href="/demo" class="flex justify-center items-center bg-transparent font-semibold bg-trasparent text-white rounded-full border-2 border-white w-[6rem] h-[3rem] hover:bg-white hover:text-black transition-all">DEMO</a>
  </div>
</template>