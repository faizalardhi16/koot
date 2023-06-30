<template>
    <div class="items-center justify-center flex flex-col p-4 text-center">
        <img :src="url" class="w-24 border border-green-500 rounded-full" />
        <h1 class="py-4 text-2xl font-bold">
            {{ name }}
        </h1>
        <p class="text-base">
            {{ description }}
        </p>
    </div>
</template>

<script>
    export default {
        props: {
           name: {
            type: String,
            required: true
           },
           description: {
            type: String,
            required: true
           },
           url: {
            type: String,
            required: true
           }
        }
    }
</script>