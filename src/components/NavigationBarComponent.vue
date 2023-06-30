<script setup>

import CustomButton from './CustomButton.vue';
    const menu = [
        {id: 1, href:"#home", title: "Home"},
        {id: 2 , href:"#features", title: "Features"},
        {id: 3, href:"#specs", title: "Specs"},
        {id: 4, href:"#review", title: "Review"},
        {id: 5, href:"#contacts", title: "Contacts"},
    ]
</script>

<template>
    <nav :class="`z-50 bg-white fixed justify-around items-center py-4 w-full flex flex-row transition ease-in duration-200`">
        <div class="w-1/4 items-center justify-center flex">
            <h1 class="text-4xl font-bold text-[#2ecc71]">koot</h1>
        </div>

        <div class="w-2/4 items-center justify-center flex">
            <a class="m-4 font-bold text-xl" :key="item.id" v-for="item in menu" :href="item.href">{{ item.title }}</a>
        </div>

        <div class="w-1/4 items-center justify-center flex">
            <CustomButton label="Buy Now" :onClick="buyNow" />
        </div>
    </nav>
</template>


<script>
    export default {
    data() {
        return {
            isTransparent: false,
        };
    },
    mounted() {
    },
    beforeUnmount() {
    },
    methods: {
        buyNow(){
            alert("CLICKED")
        }
    },
    components: { CustomButton }
}
</script>