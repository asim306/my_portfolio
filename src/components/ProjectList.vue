<template>
  <section id="projects" class="projects">
    <h2>My Projects</h2>
    <div class="project-list">
      <div v-for="(project, index) in projects" :key="index" class="project-card">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <a :href="project.link" target="_blank">View Project</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ProjectList",
  data() {
    return {
      projects: [
        { title: "Portfolio Website", description: "A personal portfolio in Vue.js", link: "#" },
        { title: "E-Commerce App", description: "Built with Flutter & Django", link: "#" },
        { title: "Hospital Management System", description: "Full-stack system with API integration", link: "#" }
      ],
    };
  },
};
</script>

<style scoped>
.projects {
  padding: 4rem;
  background: #f8f9fa;
  text-align: center;
}
.project-list {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}
.project-card {
  background: white;
  padding: 1.5rem;
  border-radius: 10px;
  width: 250px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}
</style>
