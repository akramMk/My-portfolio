<template>
  <div class="bg-[#111827] min-h-screen">
    <!-- wrap component in Suspense to handle Loading -->
    <Suspense>
      <template #default>
        <div>
          <!-- Wrap all Components inside a single root element -->
          <NavBar></NavBar>
          <HeroSection></HeroSection>
          <!-- <ServicesSection></ServicesSection> -->
          <AboutSection></AboutSection>
          <ExperienceAndSkills></ExperienceAndSkills>
          <LatestProjSection></LatestProjSection>
          <ContactSection></ContactSection>
          <FooterSection></FooterSection>
          <BackToTop></BackToTop>
        </div>
      </template>
      <template #fallback>
        <div class="flex justify-center items-center min-h-screen">
          <loadingSpinner />
        </div>
      </template>
    </Suspense>
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
const BackToTop = defineAsyncComponent(()=>import('@/components/BackToTop.vue'))
import LoadingSpinner from './components/LoadingSpinner.vue';
</script>

<style scoped>

</style>
