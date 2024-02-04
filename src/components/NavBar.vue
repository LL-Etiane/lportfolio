<script setup>

</script>

<template>
    <nav class="bg-white py-5 px-10 flex md:justify-between md:items-center">
        <a href="/" class="text-primary font-bold text-3xl">LINZY</a>

        <ul class="md:flex md:space-x-5">
            <li>
                <router-link to="/" active-class="text-primary" class="text-lg font-semibold hover:text-primary">Home</router-link>
            </li>
            <li>
                <router-link to="/about" active-class="text-primary" class="text-lg font-semibold hover:text-primary">About Me</router-link>
            </li>
            <li>
                <router-link to="/resume" active-class="text-primary" class="text-lg font-semibold hover:text-primary">Resume</router-link>
            </li>
            <li>
                <router-link to="/services" active-class="text-primary" class="text-lg font-semibold hover:text-primary">Services</router-link>
            </li>
            <li>
                <router-link to="/contact" active-class="text-primary" class="text-lg font-semibold hover:text-primary">Contact</router-link>
            </li>
        </ul>

        <ul class="md:flex md:space-x-3">
            <a href="#"><i class="fa-brands fa-x-twitter fa-lg"></i></a>
            <a href="#"><i class="fa-brands fa-linkedin fa-lg"></i></a>
            <a href="#"><i class="fa-brands fa-facebook fa-lg"></i></a>
            <a href="#"><i class="fa-brands fa-square-snapchat fa-lg"></i></a>
        </ul>
    </nav>
</template>