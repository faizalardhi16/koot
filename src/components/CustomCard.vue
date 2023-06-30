<script setup>
    defineProps({
        title: {
            type: String,
            required: true
        },
        description: {
            type: String,
            required: true
        }
    })
</script>


<template>
    <div class="w-1/3 p-4 items-center justify-center flex flex-col">   
        <h1 class="font-bold text-2xl">{{ title }}</h1>
        <p class="text-center text-base py-4">{{ description }}</p>
    </div>
</template>-

<script>

</script>