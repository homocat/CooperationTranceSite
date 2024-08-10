<script lang="ts" setup>
import Nav from './components/Nav/index.vue'
import Footer from './components/Footer/index.vue'
import BaseLayout from "./Layout/BaseLayout.vue";
</script>

<template>
  <header class="flex justify-center pt-5">
    <Nav></Nav>
  </header>
  <main class="img relative flex flex-col items-center w-screen h-auto bg-blue-950 -z-10">
    <div class="w-[100%] h-[1080px] backdrop-blur-lg"></div>
    <BaseLayout>
      <div class="absolute top-[5rem] flex flex-col justify-start backdrop-blur items-center p-5 w-[100%]">
        <router-view></router-view>
      </div>
    </BaseLayout>
    <Footer class="mt-auto"></Footer>
  </main>
</template>

<style scoped>
.img {
  position: absolute;
  top: 0;
  width: 100%;
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.16), rgba(0, 0, 0, 0) 55%, rgb(0, 0, 0)),
  radial-gradient(ellipse at center, transparent 90%, rgb(0, 0, 0)), linear-gradient(to right, rgb(0, 0, 0),
      rgba(0, 0, 0, 0), rgb(0, 0, 0)), url(./assets/uploads/background.jpg);
  background-position: 50%;
  background-repeat: no-repeat;
  background-size: cover;
}

</style>
