<script setup>
    import ContactSection from '../components/ContactSection.vue';
    import FooterSection from '../components/FooterSection.vue';
    import GetStartedSection from '../components/GetStartedSection.vue';
    import HomeSection from '../components/HomeSection.vue';
    import NavigationBarComponent from '../components/NavigationBarComponent.vue';
    import ReasonSection from "../components/ReasonSection.vue"
    import TestimonySection from "../components/TestimonySection.vue"
</script>

<template>
    <NavigationBarComponent/>

    <div class="h-[85vh] pt-24 items-center justify-center flex">
        <HomeSection />
    </div>

    <div class="items-center justify-center flex">
        <ReasonSection />
    </div>

    <div class="items-center justify-center flex my-12">
        <GetStartedSection />
    </div>
    
    <div class="items-center justify-center flex">
        <TestimonySection />
    </div>

    <div class="items-center justify-center flex">
        <ContactSection />
    </div>
    
    <div class="items-center justify-center flex">
        <FooterSection />
    </div>
</template>

