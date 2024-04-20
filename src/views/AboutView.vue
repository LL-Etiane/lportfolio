<script setup>
import linzyimg from '@/assets/images/linzy.png'
import SkillsComponent from '@/components/Skills.vue'
import TestimonialsComponent from '@/components/Testimonials.vue'

</script>

<template>
  <div class="">
    <h1 class="text-center text-primary font-bold text-2xl my-10 mb-3 underline underline-offset-8">Who am I</h1>
    <p class="text-center mx-5 md:mx-20 mt-5 md:mt-10">
      I am a highly driven and dedicated person seeking opportunities where I can fully use my skills to achieve a
      desired objective. Customer satisfaction is my top priority, I aim at working in an environment that encourages me
      to grow and succeed professionally while I utilize my skills and knowledge appropriately.
    </p>

    <section class="md:mx-10">
      <div class="flex flex-col md:flex-row mt-5 gap-1 gap-y-5 items-center px-5 md:px-10">
        <div class="md:w-[600px]">
          <img :src="linzyimg" alt="" class="h-[400px] rounded-2xl">
        </div>
        <div class="">
          <h1 class="text-primary font-bold text-xl md:text-2xl">Graphics & UI UX Designer / System Analyst</h1>
          <p class="mt-2">
            You need designs, look no further, I'm here to take that worry away. I keep to deadlines and make sure to
            deliver on time.
          </p>
          <div class="flex flex-wrap mt-7 gap-y-10">
            <div class="w-1/2">
              <h1>
                <span class="text-primary"><i class="fa-solid fa-greater-than fa-lg"></i> </span>
                <span class="font-bold"> Linkedin: </span>
                <span>Nnah Linzy</span>
              </h1>
            </div>

            <div class="w-1/2">
              <h1>
                <span class="text-primary"><i class="fa-solid fa-greater-than fa-lg"></i> </span>
                <span class="font-bold"> Degree: </span>
                <span>Bachelor's degree in Computing and Information Systems</span>
              </h1>
            </div>

            <div class="w-1/2">
              <h1>
                <span class="text-primary"><i class="fa-solid fa-greater-than fa-lg"></i> </span>
                <span class="font-bold"> City: </span>
                <span>Douala, Cameroon</span>
              </h1>
            </div>

            <div class="w-1/2">
              <h1>
                <span class="text-primary"><i class="fa-solid fa-greater-than fa-xl"></i> </span>
                <span class="font-bold"> Freelance: </span>
                <span>Available</span>
              </h1>
            </div>
          </div>

          <p class="mt-5">
            I believe in working to make sure the clients are satisfied, their satisfaction comes first. I am a great
            team work player but I also work amazingly alone. Thriving for perfection is my passion.
          </p>
          <div class="w-full mt-2 md:mt-6 flex flex-wrap space-x-5 ">
            <a href="https://twitter.com/linzy_nnah" class="block"><i class="fa-brands fa-x-twitter fa-lg"></i></a>
            <a href="https://www.linkedin.com/in/nnah-linzy-b7228020a/" class="block"><i
                class="fa-brands fa-linkedin fa-lg"></i></a>
            <a href="https://web.facebook.com/nnah.linzy.5/?_rdc=1&_rdr" class="block"><i
                class="fa-brands fa-facebook fa-lg"></i></a>
            <a href="https://www.instagram.com/linzynnah/" class="block"><i
                class="fa-brands fa-instagram fa-lg"></i></a>
            <a href="mailto:Nnahlinzy01@gmail.com" class="block"><i class="fa-solid fa-envelope fa-lg"></i></a>
          </div>
        </div>
      </div>
    </section>

    <SkillsComponent class="mt-10"/>

    <TestimonialsComponent class=""/>
  </div>
</template>