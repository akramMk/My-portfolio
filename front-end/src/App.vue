<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar></NavBar>
    <HeroSection></HeroSection>
  </div>
</template>

<script setup>
import { defineAsyncComponent } from 'vue';

const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'))
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'))

</script>

<style scoped>

</style>
