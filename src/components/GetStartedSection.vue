<script setup>

import CustomButton from './CustomButton.vue';

</script>

<template>
    <div class="w-11/12 items-center justify-around flex flex-row">
        <!---Image section-->
        <div class="w-5/12 items-center justify-center flex">
            <img src="https://m.media-amazon.com/images/I/513PuLtilUL._SX425_.jpg" class="rotate-[315deg]" />
        </div>

        <div class="w-7/12">
            <h1 class="font-bold text-justify text-5xl py-4">
                All the services we will provide you.
            </h1>

            <p class="text-justify text-xl py-4">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Suscipit, dolorem ullam tenetur voluptate optio unde. 
                Repudiandae corrupti laborum blanditiis eligendi illum provident.
            </p>

            <CustomButton label="Get Started" :onClick="getStarted" />
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                imagePath: "/headset.jpg"
            };
        },
        methods: {
            getStarted() {
                alert("CLICK")
            }
        },
        components: { CustomButton },
}
</script>