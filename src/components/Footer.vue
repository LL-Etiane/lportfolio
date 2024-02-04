<template>
    <footer class="bg-[#3A3A3A] py-10 px-20 border-t-8 border-t-[#77757599]">
        <div class="flex md:space-x-10">
            <div class="">
                <router-link to="/" class="text-white font-bold text-2xl font-roboto">Linzy</router-link>
                <ul class="md:flex md:space-x-3 text-white mt-5">
                    <a href="#"><i class="fa-brands fa-x-twitter fa-lg"></i></a>
                    <a href="#"><i class="fa-brands fa-linkedin fa-lg"></i></a>
                    <a href="#"><i class="fa-brands fa-facebook fa-lg"></i></a>
                    <a href="#"><i class="fa-brands fa-square-snapchat fa-lg"></i></a>
                </ul>
            </div>
            <ul class="md:flex w-full justify-evenly">
                <li>
                    <router-link to="/" class="text-white text-lg font-semibold hover:text-primary">Home</router-link>
                </li>
                <li>
                    <router-link to="/about" class="text-white text-lg font-semibold hover:text-primary">About Me</router-link>
                </li>
                <li>
                    <router-link to="/resume" class="text-white text-lg font-semibold hover:text-primary">Resume</router-link>
                </li>
                <li>
                    <router-link to="/services" class="text-white text-lg font-semibold hover:text-primary">Services</router-link>
                </li>
                <li>
                    <router-link to="/contact" class="text-white text-lg font-semibold hover:text-primary">Contact</router-link>
                </li>
            </ul>
        </div>
    </footer>
</template>