<script setup>
import headerBg from '@/assets/images/header.png'
import lineImg from '@/assets/images/line6.svg'

</script>

<template>
  <section :style="{ backgroundImage: `linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url(${headerBg})` }" 
  class="min-h-[100vh] w-[100vw] flex items-center bg-cover bg-center bg-no-repeat relative px-4 md:px-20"
>
    <div class="w-full md:w-[600px]">
      <div class="text-white text-6xl font-montserrat">
        <h1>Hi! I’m Linzy, UI UX</h1>
        <h1 class="text-[#ED8000] mt-3">Designer</h1>
      </div>
      <img :src="lineImg" alt="" class="mt-4">
      <p class="text-white mt-2 font-montserrat font-semibold text-xl">
        I’m a professional Graphics / UI UX Designer with a zeal to transform ideas to reality. Test my skills and find out.
      </p>
      <div class="w-full mt-10 flex flex-wrap gap-5 font-semibold">
        <router-link to="/" class="text-primary">Home</router-link>
        <router-link to="/about" class="text-white hover:text-primary">About me</router-link>
        <router-link to="/resume" class="text-white hover:text-primary">Resume</router-link>
        <router-link to="/services" class="text-white hover:text-primary">Services</router-link>
        <router-link to="/contact" class="text-white hover:text-primary">Contact</router-link>
      </div>
      <div class="w-full mt-6 flex flex-wrap space-x-5 text-white">
        <a href="https://twitter.com/linzy_nnah" class="block"><i class="fa-brands fa-x-twitter fa-lg"></i></a>
        <a href="https://www.linkedin.com/in/nnah-linzy-b7228020a/" class="block"><i class="fa-brands fa-linkedin fa-lg"></i></a>
        <a href="https://web.facebook.com/nnah.linzy.5/?_rdc=1&_rdr" class="block"><i class="fa-brands fa-facebook fa-lg"></i></a>
        <a href="https://www.instagram.com/linzynnah/" class="block"><i class="fa-brands fa-instagram fa-lg"></i></a>
        <a href="mailto:Nnahlinzy01@gmail.com" class="block"><i class="fa-solid fa-envelope fa-lg"></i></a>
      </div>
    </div>

    <div class="absolute bottom-5 right-10">
      <h1 class="text-white font-bold">Designed by <span class="text-primary">Nnah Linzy</span></h1>
    </div>
  </section>
</template>
