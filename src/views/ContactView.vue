<script setup>
import { ref } from 'vue'

const name = ref('')
const email = ref('')
const subject = ref('')
const message = ref('')

const submit = () => {
    // validate form
    if (!name.value || !email.value || !subject.value || !message.value) {
        alert('Please fill in all fields')
        return
    }

}

</script>
<template>
    <div class="">
        <div class="flex flex-col justify-center items-center mt-10">
            <h1 class="text-primary font-bold text-2xl text-center uppercase">CONTACT</h1>
            <hr class="text-primary bg-primary h-1 w-10 text-center">
        </div>
        <p class="text-center mt-3 px-3 md:px-20">
            Reach Out and Let's Make Magic Happen, Start Your Creative Journey Today. Get in Touch: I'd Love to Hear
            from You
        </p>

        <div class="flex justify-center w-full mt-10 mb-10 px-5 md:px-0">
            <div class="md:w-4/5 bg-white shadow-md shadow-primary rounded-md py-5 px-2 md:px-10">
                <div class="flex justify-between md:justify-evenly">
                    <div class="flex gap-2 items-center">
                        <div class="bg-primary bg-opacity-10 p-3 rounded-3xl">
                            <i class="fa-solid fa-location-dot fa-xl text-primary"></i>
                        </div>
                        <div class="">
                            <h1 class="text-primary uppercase">Location</h1>
                            <h1>Douala, Cameroon</h1>
                        </div>
                    </div>

                    <div class="flex gap-2 items-center">
                        <div class="bg-primary bg-opacity-10 p-3 rounded-3xl">
                            <i class="fa-solid fa-share-nodes fa-xl text-primary"></i>
                        </div>
                        <div class="">
                            <h1 class="text-primary uppercase">SOCIALS</h1>
                            <div class="flex flex-wrap space-x-5">
                                <a href="https://twitter.com/linzy_nnah" class="block"><i
                                        class="fa-brands fa-x-twitter fa-lg"></i></a>
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
                </div>

                <form action="" class="mt-10">
                    <input type="text" name="name" id="name" placeholder="Your Name" v-model="name" class="w-full py-4 px-5 bg-primary bg-opacity-10 rounded-md my-3" required>
                    <input type="email" name="email" id="email" placeholder="Your Email" v-model="email" class="w-full py-4 px-5 bg-primary bg-opacity-10 rounded-md my-3" required>
                    <input type="text" name="subject" id="subject" placeholder="Subject" v-model="subject" class="w-full py-4 px-5 bg-primary bg-opacity-10 rounded-md my-3" required>
                    <textarea name="message" id="message" cols="15" rows="10" placeholder="Message" v-model="message" class="w-full py-4 px-5 bg-primary bg-opacity-10 rounded-md my-3" required></textarea>

                    <div class="flex justify-end">
                        <button type="submit" class="bg-primary text-white font-bold py-2 px-5 rounded-xl mt-5 shadow-lg">Submit</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<style>
    input {
        border: none;
        outline: none;
    }
</style>