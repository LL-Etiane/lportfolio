<script setup>
defineProps({
    name: String,
    year: String,
    place: {
        type: String,
        default: 'London Institute of InfoTech & Professional Training'
    },
    qualification: {
        type: String,
        default: 'ABMA QUALIFICATIONS'
    }
});
</script>
<template>
    <div class="mt-10">
        <h1 class="text-primary font-bold text-lg uppercase">{{ name }}</h1>
        <p class="mt-2 inline-block bg-white text-[#3A3A3A] py-2 px-3 rounded-md">{{ year }}</p>
        <p class="mt-2 font-roboto">{{ place }}</p>
        <p class="mt-2 uppercase">{{ qualification }}</p>
    </div>
</template>