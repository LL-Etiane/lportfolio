<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);

function toggleMenu() {
    isMenuOpen.value = !isMenuOpen.value;
}
</script>

<template>
    <nav class="bg-black py-5 px-1 md:px-10 flex justify-between md:items-center relative">
        <a href="/" class="text-primary font-bold text-xl md:text-3xl">Nnah Linzy</a>

        <div class="absolute right-5 md:hidden" @click="toggleMenu">
            <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
        </div>

        <ul class="md:flex md:gap-5 mt-3 md:mt-0" :class="{'block': isMenuOpen, 'hidden': !isMenuOpen}">
            <li>
                <router-link to="/" class="text-md text-white font-semibold hover:text-primary">Home</router-link>
            </li>
            <li>
                <router-link to="/about" class="text-md text-white font-semibold hover:text-primary">About Me</router-link>
            </li>
            <li>
                <router-link to="/resume" class="text-md text-white font-semibold hover:text-primary">Resume</router-link>
            </li>
            <li>
                <router-link to="/services" class="text-md text-white font-semibold hover:text-primary">Services</router-link>
            </li>
            <li>
                <router-link to="/contact" class="text-md text-white font-semibold hover:text-primary">Contact</router-link>
            </li>
        </ul>
    </nav>
</template>