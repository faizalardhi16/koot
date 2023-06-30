<script setup>
import CustomButton from './CustomButton.vue'
</script>

<template>
    <div class="w-11/12 items-center justify-between flex flex-row">
        <div class="items-start justify-center flex flex-col w-1/2 min-h-[70vh]">
            <p class="text-6xl font-bold w-3/4 my-4">My reality is now going virtual</p>
            <h1 class="text-2xl w-3/4 my-4">
                Best in class virtual reality gera to make your everyday experience great. Go check it.
            </h1>
            <div class="my-4">
                <CustomButton label="Buy Now" :onClick="handleClick" />
            </div>
        </div>

        <div class="items-start justify-center text-justify flex w-1/2">
            <img v-bind:src="imagePath" alt="Deskripsi gambar">
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            imagePath: '/headset.jpg'
        }
    },
    methods: {
        handleClick() {
            alert('OK')
        }
    }
}
</script>
