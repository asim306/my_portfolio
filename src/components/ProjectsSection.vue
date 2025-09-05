<template>
  <section id="projects" class="projects-section">
    <div class="container">
      <h2 class="section-title">Projects</h2>
      
      <div class="projects-grid">
        <div 
          v-for="project in projects" 
          :key="project.title"
          class="project-card"
        >
          <img :src="project.image" alt="" class="project-image" />
          <div class="overlay">
            <h3 class="project-title">{{ project.title }}</h3>
            <p class="project-desc">{{ project.description }}</p>
            <a :href="project.link" target="_blank" class="project-link">View Project →</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import logoImg from '@/assets/logo.png'
// import portfolioImg from '@/assets/portfolio.png'
// import ecommerceImg from '@/assets/ecommerce.png'

const projects = [
  { 
    title: 'Portfolio Website', 
    description: 'Built with Vue 3 + TailwindCSS. Responsive and modern UI.', 
    link: '#', 
    image: logoImg
  },
  { 
    title: 'E-Commerce App', 
    description: 'Online shopping platform with cart and payment integration.', 
    link: '#', 
    image: logoImg
  },
  { 
    title: 'Company Logo Project', 
    description: 'Branding project showcasing a clean and modern logo design.', 
    link: '#', 
    image: logoImg   // using logo.png from assets
  },
]
</script>

<style scoped>
.projects-section {
  padding: 6rem 2rem;
  margin-top: 6rem;
  margin-bottom: 6rem;
  background: #111;
  color: white;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.section-title {
  font-size: 3rem;
  font-weight: bold;
  text-align: center;
  margin-bottom: 4rem;
  color: #facc15; /* yellow accent */
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.project-card {
  position: relative;
  border-radius: 1.5rem;
  overflow: hidden;
  box-shadow: 0 10px 25px rgba(0,0,0,0.4);
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 2px solid #fff;
}

.project-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 30px rgba(0,0,0,0.6);
}

.project-image {
  width: 100%;
  height: 220px;
  object-fit: cover;
  display: block;
  transition: transform 0.5s ease;
}

.project-card:hover .project-image {
  transform: scale(1.1);
}

.overlay {
  position: absolute;
  inset: 0;
  background-color: rgba(0, 0, 0, 0.6);
  opacity: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 2rem;
  transition: opacity 0.5s ease;
}

.project-card:hover .overlay {
  opacity: 1;
}

.project-title {
  font-size: 1.75rem;
  font-weight: bold;
  margin-bottom: 0.5rem;
}

.project-desc {
  font-size: 1rem;
  margin-bottom: 1rem;
  color: #e5e7eb;
}

.project-link {
  font-size: 1rem;
  color: #10b981;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s ease;
}

.project-link:hover {
  color: #6ee7b7;
}
</style>
