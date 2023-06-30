<script setup>
    import CardWithImage from "../components/CardWithImage.vue"
    const data = [
        {id: 1, url: "https://m.media-amazon.com/images/I/513PuLtilUL._SX425_.jpg", name: "Alexander Sorloth", description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus aliquam totam esse! Nemo autem facilis unde beatae cupiditate nobis molestiae quia. Modi nulla temporibus similique autem commodi odit recusandae nam! Lorem, ipsum."},
        {id: 2, url: "https://m.media-amazon.com/images/I/513PuLtilUL._SX425_.jpg", name: "Erling Haaland", description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus aliquam totam esse! Nemo autem facilis unde beatae cupiditate nobis molestiae quia. Modi nulla temporibus similique autem commodi odit recusandae nam! Lorem, ipsum."},
        {id: 3, url: "https://m.media-amazon.com/images/I/513PuLtilUL._SX425_.jpg", name: "Dominik Sbozszlai", description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus aliquam totam esse! Nemo autem facilis unde beatae cupiditate nobis molestiae quia. Modi nulla temporibus similique autem commodi odit recusandae nam! Lorem, ipsum."}
    ]

</script>

<template>
    <div class="w-11/12 items-center justify-center flex flex-col my-16">
        <h1 class="text-4xl font-bold text-center">
            What Our Client Says
        </h1>
        <p class="text-center w-1/3 text-xl my-4">
            Lorem ipsum dolor sit ametconsectetur adipisicing elit.
            Neque, vel? Lorem ipsum dolor sit amet.
        </p>

        <div class="items-center justify-around flex flex-row">
            <CardWithImage 
                v-for="item in data" 
                :key="item.id" 
                :name="item.name" 
                :url="item.url"
                :description="item.description"
            />
        </div>
    </div>
</template>