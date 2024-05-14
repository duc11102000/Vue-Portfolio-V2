<template>
  <div>
    <Header />
    <ProfileSection />
    <AboutSection />
    <ExperienceSection />
    <ProjectsSection />
    <ContactSection />
    <Footer />
  </div>
</template>

<script setup lang="ts">
import Header from "./Layout/Header.vue";
import ProfileSection from "@/components/Sections/ProfileSection.vue";
import AboutSection from '@/components/Sections/AboutSection.vue'
import ExperienceSection from '@/components/Sections/ExperienceSection.vue'
import ProjectsSection from "../components/Sections/ProjectsSection.vue";
import ContactSection from "../components/Sections/ContactSection.vue";
import Footer from "./Layout/Footer.vue";
</script>
