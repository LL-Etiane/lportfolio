<script setup>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

</script>

<template>
  <div class="flex flex-col min-h-screen">

    <NavBar v-if="$route.name != 'home'"/>

    <div class="flex-grow">
      <RouterView />
    </div>

    <Footer v-if="$route.name !== 'home' && $route.name !== 'resume'" class="w-full" />

  </div>
</template>