<script setup>
import headerBg from '@/assets/images/header.png'
import lineImg from '@/assets/images/line6.svg'
import profileU from '@/assets/images/ProfileU.png'
import Rectangle35 from '@/assets/images/Rectangle35.png'

</script>

<template>
  <section :style="{ backgroundImage: `linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url(${headerBg})` }" 
  class="min-h-[100vh] w-[100vw] flex items-center bg-cover bg-center bg-no-repeat relative px-4 md:px-20"
>
    <div class="w-full md:w-[600px]">
      <div class="text-white text-6xl font-montserrat">
        <h1>Hi! I’m Linzy, UI UX</h1>
        <h1 class="text-[#ED8000] mt-2">Designer</h1>
      </div>
      <img :src="lineImg" alt="" class="mt-2">
      <p class="text-white mt-2 font-montserrat font-semibold text-xl">
        I’m a professional Graphics / UI UX Designer with a zeal to transform ideas to reality. Test my skills and find out.
      </p>
      <div class="w-full mt-10 flex flex-wrap gap-5 font-semibold">
        <router-link to="/" class="text-primary">Home</router-link>
        <router-link to="/bout" class="text-white hover:text-primary">About me</router-link>
        <router-link to="/" class="text-white hover:text-primary">Resume</router-link>
        <router-link to="/" class="text-white hover:text-primary">Services</router-link>
        <router-link to="/" class="text-white hover:text-primary">Contact</router-link>
      </div>
      <div class="w-full mt-6 flex flex-wrap space-x-5 text-white">
        <a href="https://twitter.com/linzy_nnah" class="block"><i class="fa-brands fa-x-twitter fa-lg"></i></a>
        <a href="https://www.linkedin.com/in/nnah-linzy-b7228020a/" class="block"><i class="fa-brands fa-linkedin fa-lg"></i></a>
        <a href="https://web.facebook.com/nnah.linzy.5/?_rdc=1&_rdr" class="block"><i class="fa-brands fa-facebook fa-lg"></i></a>
        <a href="https://www.instagram.com/linzynnah/" class="block"><i class="fa-brands fa-instagram fa-lg"></i></a>
      </div>
    </div>

    <div class="absolute bottom-5 right-10">
      <h1 class="text-white font-bold">Designed by <span class="text-primary">Nnah Linzy</span></h1>
    </div>
  </section>

  <!-- <section class="container mt-10 flex flex-col justify-center items-center">
    <h1 class="text-[#4E018B] font-bold text-2xl uppercase text-center">INNOVATION AND ME</h1>
    <div class="flex items-start w-[70%] mt-5">
      <div class="w-1/2">
        <div class="">
          <img :src="profileU" alt="" class="h-[400px]">
        </div>
      </div>
      <div class="w-1/2 pt-16">
        <p class="text-[#4E018B] text-lg font-roboto">
          Unlock the door to creativity and innovation. Connect with me now to discuss how we can elevate your projects to new 
          heights!
        </p>
        <div class="mt-10">
          <a href="#" class="py-2 px-3 rounded-[20px] text-[#4E018B] border border-[#4E018B] font-bold">Connect</a>
        </div>
      </div>
    </div>
  </section>

  <section
  :style="{ backgroundImage: `url(${Rectangle35})` }" 
   class=" mt-10 py-20 px-20 bg-cover bg-center bg-no-repeat relative mb-10"
  >
    <div value="">
      <p class="text-white w-[300px] font-roboto text-xl leading-10">
        From Flyers to Website to Mobile Apps to Dashboards, you name it, I <span class="text-[#ED8000]">Design</span> it.
      </p>

      <div class="mt-8">
        <div class="inline-block align-middle">
          <router-link to="" class="text-white font-roboto text-xl">Resume</router-link>
          <hr class="w-full">
        </div>
      </div>
    </div>
  </section> -->
</template>
