<script setup>
import { ref } from 'vue';
import skillbg from '@/assets/images/skills.png';

const skills = ref([
    { name: 'HTML', percentage: 90 },
    { name: 'CSS', percentage: 80 },
    { name: 'JavaScript', percentage: 70 },
    { name: 'Digital Marketing', percentage: 60 },
    { name: 'Wordpress', percentage: 65 },
    { name: 'Graphics Design', percentage: 95 },
    { name: 'Project Management', percentage: 30 },
    { name: 'Copywriting', percentage: 65 },
    { name: 'Figma', percentage: 90 },
    { name: 'UI UX Design', percentage: 100 },
]);
</script>

<template>
    <div :style="{ backgroundImage: `linear-gradient( rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.5) ), url(${skillbg})` }" class="skills bg-no-repeat bg-cover py-10 px-10 text-white">
        <h1 class="text-primary text-center text-2xl uppercase font-bold underline underline-offset-8">Skills</h1>
        <p class="mt-5 text-center">
            These skills are some of my top skills I have acquired and they will help give you a brief overview of the many ways I can use them to make your ideas become reality and just with the right budget. 
        </p>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-5 mt-10">
            <div v-for="skill in skills" :key="skill.name" class="p-5 rounded-lg">
                <div class="flex justify-between text-white font-bold">
                    <h1>{{ skill.name }}</h1>
                    <h1>{{ skill.percentage }}%</h1>
                </div>
                <div class="w-full bg-white bg-opacity-20 mt-4 rounded-lg">
                    <div :style="{ width: skill.percentage + '%' }" class="bg-primary h-2 rounded-lg"></div>
                </div>
            </div>
        </div>  
    </div>
</template>