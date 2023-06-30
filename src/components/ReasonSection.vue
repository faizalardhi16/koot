<script setup>
import CustomCard from './CustomCard.vue';

    const data = [
        {id: 1, title: "Easy to Use", description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus aliquam totam esse! Nemo autem facilis unde beatae cupiditate nobis molestiae quia. Modi nulla temporibus similique autem commodi odit recusandae nam! Lorem, ipsum."},
        {id: 2, title: "High Quality", description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus aliquam totam esse! Nemo autem facilis unde beatae cupiditate nobis molestiae quia. Modi nulla temporibus similique autem commodi odit recusandae nam! Lorem, ipsum."},
        {id: 3, title: "Best In Market", description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus aliquam totam esse! Nemo autem facilis unde beatae cupiditate nobis molestiae quia. Modi nulla temporibus similique autem commodi odit recusandae nam! Lorem, ipsum."},
    ]
</script>

<template>
   <div class="w-11/12 justify-center items-center flex flex-col">
        <h1 class="font-bold text-3xl">Why Choose Us?</h1>

        <div class="mt-[23px] flex flex-row items-center justify-around w-full">
            <CustomCard v-for="item in data" :key="item.id"  :title="item.title" :description="item.description"/>
        </div>
        
   </div>
</template>
