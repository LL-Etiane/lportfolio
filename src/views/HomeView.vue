<script setup>
import headerBg from '@/assets/images/header.png'
import lineImg from '@/assets/images/line6.svg'
import profileU from '@/assets/images/ProfileU.png'
import Rectangle35 from '@/assets/images/Rectangle35.png'

</script>

<template>
  <header :style="{ backgroundImage: `linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url(${headerBg})` }" 
  class="min-h-[70vh] flex items-center bg-cover bg-center bg-no-repeat relative px-20"
  >
    <div class="md:w-[500px]">
      <h1 class="text-white text-6xl font-montserrat">
        <span>Hi! I’m Linzy</span> <br />
        <span>UI UX <span class="text-[#ED8000]">Designer</span></span>
      </h1>
      <img :src="lineImg" alt="" class="mt-2">
      <p class="text-white mt-2 font-montserrat font-semibold text-xl">
        I’m a professional Graphics / UI UX Designer with a zeal to transform ideas to reality. Test my skills and find out.
      </p>
      <div class="mt-5 flex space-x-5">
        <a href="#" class="py-2 px-3 rounded-[20px] text-white border border-white">Find out more</a>
        <a href="#" class="py-2 px-3 rounded-[20px] text-white border bg-primary border-primary">Hire me button</a>
      </div>
    </div>
  </header>

  <section class="container mt-10 flex flex-col justify-center items-center">
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
  </section>
</template>
