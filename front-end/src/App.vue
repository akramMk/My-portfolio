<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar></NavBar>
    <HeroSection></HeroSection>
    <ServicesSection></ServicesSection>
  </div>
</template>

<script setup>
import { defineAsyncComponent } from 'vue';

const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'))
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'))
const ServicesSection = defineAsyncComponent(()=>import('@/components/ServicesSection.vue'))
</script>

<style scoped>

</style>
