<!-- <template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style> -->


<template>
  <div id="app">
    <AppNavbar />
    <HeroBanner />
    <AboutSection />
    <ProjectList />
    <ContactSection />
  </div>
</template>

<script>
import AppNavbar from "./components/AppNavbar.vue";
import HeroBanner from "./components/HeroBanner.vue";
import AboutSection from "./components/AboutSection.vue";
import ProjectList from "./components/ProjectList.vue";
import ContactSection from "./components/ContactSection.vue";

export default {
  name: "App",
  components: { AppNavbar, HeroBanner, AboutSection, ProjectList, ContactSection },
};
</script>
