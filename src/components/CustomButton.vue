<template>
    <button @click="onClick" class="custom-button 
        text-base font-bold 
        text-white bg-[#2ecc71] p-2 rounded-xl hover:bg-[#27ae60]
        transition duration-200
    ">{{ label }}</button>
</template>

<script>
    export default{
        props:{
            label:{
                type: String,
                required: true
            },
            onClick: {
                type: Function,
                required: true
            }
        },
        methods: {
     
        }
    }
</script>


