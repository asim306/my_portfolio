<template>
  <div class="app-container font-sans text-white">
    <!-- Sidebar -->
    <SideBar />

    <!-- Main content -->
    <main class="w-full space-y-40">
      <!-- <HeroSection id="hero" /> -->
      <AboutSection id="about" />
      <SkillsSection id="skills" />
      <ProjectsSection id="projects" />
      <ContactSection id="contact" />
    </main>
  </div>
</template>

<script>
import SideBar from '@/components/SideBar.vue'
// import HeroSection from '@/components/HeroSection.vue'
import AboutSection from '@/components/AboutSection.vue'
import SkillsSection from '@/components/SkillsSection.vue'
import ProjectsSection from '@/components/ProjectsSection.vue'
import ContactSection from '@/components/ContactSection.vue'

export default {
  name: 'App',
  components: {
    SideBar,
    // HeroSection,
    AboutSection,
    SkillsSection,
    ProjectsSection,
    ContactSection
  }
}
</script>

<style>
.app-container {
  /* display: flex; */
  background: linear-gradient(to bottom, #52648f, #63799c); /* dark gradient background */
  min-height: 100vh;
}
/* Push main content to the right of sidebar */
.ml-20 {
  margin-left: 80px; /* matches sidebar width */
}

/* Smooth scrolling for anchor links */
html {
  scroll-behavior: smooth;
}
</style>
