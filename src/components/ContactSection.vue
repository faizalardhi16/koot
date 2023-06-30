<template>
    <div class="w-11/12 items-center justify-center flex flex-col">
        <h1 class="font-bold text-6xl text-center">Contact Us</h1>

        <form method="POST" @submit="handleSubmit" class="bg-[#2d3436] w-2/3 my-8 items-center justify-center flex flex-col py-8">
            <input type="text" :value="name" 
                class="w-3/4 h-12 outline-none p-2 rounded-md my-4" 
                placeholder="Name"
                @change="onChange"
                name="name"
            />
            <input type="email" 
                required 
                :value="email" 
                class="w-3/4 h-12 outline-none p-2 rounded-md my-4" 
                placeholder="Email"
                name="email"
                @change="onChange"
            />
            <input 
                type="text" 
                :value="message" 
                class="w-3/4 h-12 outline-none p-2 rounded-md my-4" 
                placeholder="Message"
                name="message"
                @change="onChange"
            />

            <button type="submit" class="my-4 bg-white w-3/4 p-4 rounded-md 
            hover:bg-[#2ecc71] transition duration-200 hover:text-white text-base
            ">Submit</button>
        </form>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                name: "",
                email: "",
                message: ""
            }
        },  
        methods: {
            onChange(e){
                this[e.target.name] = e.target.value
            },
            handleSubmit(e){
                e.preventDefault()
                const obj = {
                    name: this.name,
                    email: this.email,
                    message:this.message
                }

                console.log(obj)
            }
        }
    }
</script>