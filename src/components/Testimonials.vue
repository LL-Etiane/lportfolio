<script setup>
import { ref } from 'vue';

const testimonials = ref([
    { name: 'Sam', image: 'https://s3-alpha-sig.figma.com/img/5209/3bd4/d799d9dcdef8bed39a1a5c13b8b1653c?Expires=1711929600&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=awJSj4nF6CXJlSx9mV2rHmWG1jC1xpMvIkptuHN752P8Y68-qef73tshTt1JRxw30n5CeYD-gmXlZ3VVfxYcrCV3ZhInjcMQgWddzzC3LJLTZuPnpxwrvOQbDcmOF~fLaeGpJ1olJ0LXr9-6MlJpo7WHQKvEK7mOsHRnRX7Y242DgpvzdtGrev-tt~Q1s10PDnM0A3EByPRzRoh4ypN769S0zWq-ID0d3TDvlQ4xxmttGoqRNSoPL9oDrGBnDoN3gvSlEaZaWC18jsJO8FaYXRkmONNP1mhnMLkjSAviqb4oQeE2l7hxhmc9oOshK~avi3cI0Ab~qSyiEnwqHCJ1Cw__', message: 'Linzy made my dream business card and I couldn’t help but ask her to design my flyers and all my designs.' },
    { name: 'Jane', image: 'https://s3-alpha-sig.figma.com/img/2cf2/8529/c55d9beef148505189ec77359141ede7?Expires=1711929600&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=Q6Rz0udEjinL6bkyrZ0~8LNJnumV0IumzPfzoTXWhXhS5nBSimMDnf6oRkKPsH7Ln1ivGZNbG52N-V-d7mPuT69qLvTwvk6WaMj5ePH2tXa6kHeG93j8ffG~ewdx4wTNnJwwW8p7NWu1lM9y5RnGnttPVjF0Xg3HrteXK4fP6IjjfpCy-g-9J8y023X4TlWYeTnr2yFiWnT9HXT8aRda0LXT855AKLDzn7tXh~ufOt-gnqU8TUemtS9n6FCMXJGC-ZRevKoOW1wSDK2S7XaMfylQdlR-5MKxxFz7M5jsd2n8Gh0Qz8rZeeFQoWe-WoMSnqfPYxt5wTgyyV7ylOQrNg__', message: 'I love the designs Linzy Created for my business flyers. They were amazing' },
    { name: 'John', image: 'https://s3-alpha-sig.figma.com/img/8fe7/ad6b/85c053224d98bfd7e680608c07f3c239?Expires=1711929600&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=aNXqJ1lfv2lkN9zyEpzWFCXpVXsS3scfV~mKu7kiVerU3DBLoNkHlQWeCBcJe57bIob2HTCEc9Npy3E8jXiUWYQWDpXV1adzanuK4bUh5b4My8poD8TjwXSA7idsZ04K9PzJeWPnxufdavJPuh1UsxX5oxpTA7rNyQ5rB9GzJXn0ToVJKlBqYd9dqSyI178p0MCKWuYvIvIAqAwC7dMHMoK5GVyHWGXC7~tucuxR7stfX7Aip~RNfPyxahFlfwul-M78FsFc5O63QblI6CzGBUp2h3Kkihs1LuIal-AN67XjnSfuMoI6Pn-pcg0y3UkyB-t0ASyASW31BVDyP8b~4A__', message: 'She handles everything given to her with so much ease.' },
])
</script>
<template>
    <div class="container mx-auto py-10">
        <div class="flex flex-col justify-center items-center">
            <h1 class="text-primary font-bold text-2xl text-center">TESTIMONIALS</h1>
            <hr class="text-primary bg-primary h-1 w-10 text-center">
        </div>
        <p class="mt-2 text-center">
            A few things people have to say about my work. But don’t take their words for it. Go ahead and give me a try
        </p>

        <div class="flex flex-col md:flex-row justify-center mt-10 px-5">
            <div v-for="(testimonial,index) in testimonials" :key="testimonial.name" :class="{'testimonial_shadow z-50':index%2 != 0}" class="py-5 px-10 md:w-[300px] rounded-[40px] bg-white flex flex-col justify-center items-center">
                <img :src="`${testimonial.image}`" alt="" class="h-20 w-20 rounded-full">
                <h1 class="font-bold text-xl mt-2">{{ testimonial.name }}</h1>
                <p class="text-center">
                    {{ testimonial.message }}
                </p>
            </div>
        </div>
    </div>
</template>