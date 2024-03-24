<script setup>
import { ref } from 'vue'
import headerBg from '@/assets/images/header3.png'
import icon1 from '@/assets/images/icon1.png'
import icon2 from '@/assets/images/icon2.png'
import icon3 from '@/assets/images/icon3.png'
import icon4 from '@/assets/images/icon4.png'
import icon5 from '@/assets/images/icon5.png'
import icon6 from '@/assets/images/icon6.png'

const services = ref([
    {
        icon: icon1,
        title: 'UI UX Design',
        description: 'Crafting Seamless Experiences and Unlocking Digital Delight.'
    },
    {
        icon: icon2,
        title: 'Business Analysis',
        description: 'Empowering Growth through Insights by unleashing your business potential.'
    },
    {
        icon: icon3,
        title: 'Copywriting',
        description: "It's a journey, and we're here to empower you every step of the way."
    },
    {
        icon: icon4,
        title: 'Portfolio Design & Development',
        description: 'Designing Your Success Story: Showcasing Creativity and Impact.'
    },
    {
        icon: icon5,
        title: 'Digital Marketing Consultant',
        description: 'Elevate your online presence with expert guidance from a seasoned digital marketing consultant.'
    },
    {
        icon: icon6,
        title: 'Graphics Design',
        description: 'Transforming Ideas into Visual Masterpieces: Elevate Your Brand with Exceptional Graphics Designs.'
    }
])

</script>

<template>
    <section :style="{ backgroundImage: `linear-gradient( rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.5) ), url(${headerBg})` }"
        class="min-h-[100vh] bg-cover bg-center bg-no-repeat relative">
        <div class="px-4 md:px-20 pt-5 text-white">
            <div class="flex flex-col justify-center items-center">
                <h1 class="text-primary font-bold text-2xl text-center">What I offer</h1>
                <hr class="text-primary bg-primary h-1 w-10 text-center">
            </div>
            <p class="text-center mt-10 px-3 md:px-20">
                Welcome to Nnah LInzy’s portfolio of services. I specialize in UI UX Design, web development and
                business analysis, offering tailored solutions for businesses and individuals to establish a compelling
                online presence and drive sustainable growth.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-5 mt-10">
                <div
                    v-for="(service, index) in services"
                    :key="index"
                    class="bg-black bg-opacity-60 flex flex-col justify-center items-center py-3 px-10 service_box">
                    <div class="bg-primary img-shadow rounded-full p-5">
                        <img :src="service.icon" alt="icon1" class="w-10 h-10">
                    </div>
                    <h1 class="text-primary font-bold mt-2 hover:text-white">{{ service.title }}</h1>
                    <p class="font-roboto text-center font-extralight mt-2">{{ service.description }}</p>
                </div>
            </div>
        </div>

        <section class="bg-black py-5 mt-10">
            <h1 class="text-white text-center text-2xl">Let’s Get in Touch</h1>
        </section>

        <div class="pr-2 md:pr-20 py-5">
            <h1 class="text-white font-bold text-end">Designed by <span class="text-primary">Nnah Linzy</span></h1>
        </div>
    </section>
</template>

<style>
.img-shadow {
    -webkit-box-shadow: 12px -5px 25px -4px rgba(237,128,0,1);
-moz-box-shadow: 12px -5px 25px -4px rgba(237,128,0,1);
box-shadow: 12px -5px 25px -4px rgba(237,128,0,1);
}

.service_box {
    transition: background-color 0.3s ease; 
}

.service_box h1 {
    transition: color 0.3s ease; 
}

.service_box .img-shadow {
    transition: box-shadow 0.3s ease; 
}

.service_box:hover {
    background-color: #ED8000;
}

.service_box:hover h1 {
    color: white;
}

.service_box:hover .img-shadow {
    -webkit-box-shadow: 12px -5px 25px -4px rgba(255,255,255,1);   
    -moz-box-shadow: 12px -5px 25px -4px rgba(255,255,255,1);
    box-shadow: 12px -5px 25px -4px rgba(255,255,255,1);
}


</style>
