<script setup>
import { ref } from 'vue';
import headerBg from '@/assets/images/header2.png'
import EducationComponent from '@/components/Education.vue'
import Footer from '@/components/Footer.vue';

const education = ref([
    { name: 'LEVEL 6 DIPLOMA IN COMPUTING AND INFORMATION SYSTEMS', year: '2022 - 2023', place: 'London Institute of InfoTech & Professional Training', qualification: 'ABMA QUALIFICATIONS' },
    { name: 'LEVEL 5 DIPLOMA IN COMPUTING AND INFORMATION SYSTEMS', year: '2021 - 2022', place: 'London Institute of InfoTech & Professional Training', qualification: 'ABMA QUALIFICATIONS' },
    { name: 'LEVEL 4 DIPLOMA IN COMPUTING AND INFORMATION SYSTEMS', year: '2020 - 2021', place: 'London Institute of InfoTech & Professional Training', qualification: 'ABMA QUALIFICATIONS' },
    { name: 'GCE ADVANCED LEVEL (A Levels)', year: '2019', place: 'Goverment High Schol Bonadikombo (GHS)', qualification: ''},
    { name: 'GCE ORDINARY LEVEL (O Levels)', year: '2017', place: 'Goverment High Schol Bonadikombo (GHS)', qualification: ''}
]);

</script>
<template>
    <div :style="{ backgroundImage: `url(${headerBg})` }" class="min-h-[100vh] md:min-h-[100vh] overflow-auto bg-cover bg-scroll bg-center bg-no-repeat relative">
        
        <div class="mt-3 w-full">
            <div class="px-3 md:px-36">
                <section class="bg-black bg-opacity-80 text-white w-full py-3 px-5 rounded-lg mb-4">
                    <div class="flex flex-col justify-center items-center">
                        <h1 class="text-primary font-bold text-2xl text-center uppercase">Resume</h1>
                        <hr class="text-primary bg-primary h-1 w-10 text-center">
                    </div>
                    <p class="text-center mt-10 px-5 md:px-20">
                        Here is a little summary about my qualification but these qualifications are only what is on
                        paper
                        for I possess more than they say. And if you do not believe me, I am up for a trial.
                    </p>
                    <div class="mt-20 grid grid-cols-1 md:grid-cols-2 gap-3">
                        <div class="">
                            <h1 class="text-primary font-bold text-xl uppercase">Summary</h1>
                            <div class="mt-4 border-l-2 border-l-primary pl-5">
                                <h1 class="text-primary font-bold text-lg uppercase">Nnah Linzy</h1>
                                <p class="text-left font-roboto mt-3">
                                    Nnah Linzy is a holder of a bachelors degree in Computing and Information Systems.
                                    With
                                    a one year in secretarial duty. I am goal driven, creative, a fast learner, a
                                    critical
                                    thinker and I work well alone as well as in a team. Specialized in Computing and
                                    information systems with good copywriting skills and able to generate solutions in
                                    stressful situations.
                                </p>
                                <p class="mt-3">Douala, Cameroon</p>
                            </div>

                            <div class="mt-20">
                                <h1 class="text-primary font-bold text-xl uppercase">Education</h1>
                                <div class="border-l-2 border-l-primary pl-5">
                                    <EducationComponent v-for="edu in education" :key="edu.name" :name="edu.name"
                                        :year="edu.year" :place="edu.place" :qualification="edu.qualification" />
                                </div>
                            </div>
                        </div>
                        <div class="">
                            <h1 class="text-primary font-bold text-xl uppercase">Professional Experience</h1>
                            <div class="mt-4 border-l-2 border-l-primary pl-5">
                                <h1 class="text-primary font-bold text-lg uppercase">PRODUCT DESIGNER</h1>
                                <p class="mt-2 inline-block bg-white text-[#3A3A3A] py-2 px-3 rounded-md">2023 - Present
                                </p>
                                <h1 class="mt-2">MYTECHGENUIS (MTG)</h1>
                                <ul class="font-roboto mt-3 list-disc pl-5 space-y-2">
                                    <li>Design websites</li>
                                    <li>Design dashboards</li>
                                    <li>Design mobile apps</li>
                                    <li>Conducted user research</li>
                                    <li>Created user persona</li>
                                    <li>Work with developers to come up with the exact designs</li>
                                    <li>Attended regular meetings to discuss on the project's progress</li>
                                </ul>
                            </div>

                            <div class="mt-10 border-l-2 border-l-primary pl-5">
                                <h1 class="text-primary font-bold text-lg uppercase">GRAPHICS DESIGNER</h1>
                                <p class="mt-2 inline-block bg-white text-[#3A3A3A] py-2 px-3 rounded-md">2023 - Present
                                </p>
                                <h1 class="mt-2">FREELANCE</h1>
                                <ul class="font-roboto mt-3 list-disc pl-5 space-y-2">
                                    <li>Developed numerous marketing programs (logos, banners & flyers).</li>
                                    <li>Managed up to 5 projects or tasks at a given time while under pressure.</li>
                                    <li>Recommended and consulted with clients on the most appropriate graphics designs.
                                    </li>
                                </ul>
                            </div>

                            <div class="mt-10 border-l-2 border-l-primary pl-5">
                                <h1 class="text-primary font-bold text-lg uppercase">BUSINESS ANALYST INTERNSHIP</h1>
                                <p class="mt-2 inline-block bg-white text-[#3A3A3A] py-2 px-3 rounded-md">2023</p>
                                <h1 class="mt-2">VISIONARY TECHNOLOGIES COMPANY (VTC)</h1>
                                <ul class="font-roboto mt-3 list-disc pl-5 space-y-2">
                                    <li>Conducted competitive analysis of businesses</li>
                                    <li>Prepare project proposals</li>
                                    <li>Prepared scope of work</li>
                                    <li>Conducted lead generation</li>
                                    <li>Set up email Campaigns</li>
                                    <li>Create Flyers</li>
                                    <li>Draw up Software requirement specification document and website specification
                                        document</li>
                                    <li>Assisted in recruitment</li>
                                    <li>Content Gathering</li>
                                </ul>
                            </div>

                            <div class="mt-10 border-l-2 border-l-primary pl-5">
                                <h1 class="text-primary font-bold text-lg uppercase">SECRETARY</h1>
                                <p class="mt-2 inline-block bg-white text-[#3A3A3A] py-2 px-3 rounded-md">2019 - 2020
                                </p>
                                <h1 class="mt-2">MENGOVIC</h1>
                                <ul class="font-roboto mt-3 list-disc pl-5 space-y-2">
                                    <li>Help clients choose the products they want</li>
                                    <li>Produce weekly reports</li>
                                    <li>Making sure clients have a favourable experience while with us.</li>
                                    <li>Taking stock</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="flex justify-center my-3">
                        <a href="https://drive.google.com/file/d/1YBieTVAK0RNnMSQYUTF8vN-p3gFr0z3O/view?usp=sharing" target="_blank" class="mt-2 inline-block bg-primary text-sm text-white font-bold py-2 px-3 rounded-md hover:bg-white hover:text-primary transition-colors duration-500 ease-in-out">Download Resume</a>
                    </div>
                </section>
            </div>
        </div>
    </div>
</template>