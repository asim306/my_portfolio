<template>
  <div class="app-container font-sans text-white flex">
    <!-- Sidebar on the left -->
    <div class="sidebar-container">
      <SideBar />
    </div>

    <!-- Blank space -->
    <div class="spacer"></div>

    <!-- Main content -->
    <main class="main-content space-y-40">
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
  display: flex;
  flex-direction: row; /* horizontal layout */
  background: linear-gradient(to bottom, #393d3d, #869292);
  min-height: 100vh;
  width: 100%;
}

/* Sidebar container */
.sidebar-container {
  flex-shrink: 0;
}

/* Blank space between sidebar and content */
.spacer {
  width: 300px; /* adjust this gap as needed */
}

/* Main content */
.main-content {
  flex: 1;
  padding: 2rem;
}

html {
  scroll-behavior: smooth;
}
</style>
