<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar></NavBar>
    <HeroSection></HeroSection>
    <!-- <ServicesSection></ServicesSection> -->
    <AboutSection></AboutSection>
    <ExperienceAndSkills></ExperienceAndSkills>
    <LatestProjSection></LatestProjSection>
    <ContactSection></ContactSection>
    <FooterSection></FooterSection>
  </div>
</template>

<script setup>
import { defineAsyncComponent } from 'vue';

const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'))
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'))
// const ServicesSection = defineAsyncComponent(()=>import('@/components/ServicesSection.vue'))
const AboutSection = defineAsyncComponent(()=>import('@/components/AboutSection.vue'))
const ExperienceAndSkills = defineAsyncComponent(()=>import('@/components/ExperienceAndSkills.vue'))
const LatestProjSection = defineAsyncComponent(()=>import('@/components/LetesProjSection.vue'))
const ContactSection = defineAsyncComponent(()=>import('@/components/ContactSection.vue'))
const FooterSection = defineAsyncComponent(()=>import('@/components/FooterSection.vue'))
</script>

<style scoped>

</style>
