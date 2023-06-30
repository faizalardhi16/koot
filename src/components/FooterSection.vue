<script setup>
    const date = new Date()
    const year = date.getFullYear()
</script>

<template>
    <div class="w-11/12 items-center justify-center flex bg-[#2d3436] my-4 min-h-[5vh]">
        <p class="text-white">&copy; {{ year }} Copyrights koot.com all rights reserved</p>
    </div>
</template>