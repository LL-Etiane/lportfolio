<script setup>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

</script>

<template>
  <div class="flex flex-col min-h-screen">

    <NavBar />

    <div class="flex-grow">
      <RouterView />
    </div>

    <Footer class="w-full" />

  </div>
</template>