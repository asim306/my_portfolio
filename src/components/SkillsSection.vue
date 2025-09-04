<template>
    <section id="skills" class="skills-section">
      <div class="container">
        <h2 class="section-title">Skills</h2>
  
        <div class="skills-grid">
          <div
            v-for="skill in skills"
            :key="skill.name"
            class="skill-card"
            :style="{ background: skill.cardGradient }"
          >
            <div class="skill-header">
              <span class="skill-icon">{{ skill.icon }}</span>
              <h3 class="skill-name">{{ skill.name }}</h3>
            </div>
  
            <!-- Progress bar -->
            <div class="progress-bar">
              <div
                class="progress-fill"
                :style="{ width: skill.level + '%', background: skill.barGradient }"
              ></div>
            </div>
  
            <p class="skill-level">{{ skill.level }}%</p>
            <p class="skill-desc">{{ skill.description }}</p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  const skills = [
    {
      name: 'Vue.js',
      level: 95,
      icon: '🖖',
      description: 'Building reactive frontend apps with Vue 2 & 3.',
      cardGradient: 'linear-gradient(to right, #42b883, #35495e)',
      barGradient: 'linear-gradient(to right, #42b883, #3a7bd5)'
    },
    {
      name: 'JavaScript',
      level: 90,
      icon: '✨',
      description: 'Strong JS fundamentals for web development.',
      cardGradient: 'linear-gradient(to right, #f0db4f, #f7df1e)',
      barGradient: 'linear-gradient(to right, #f0db4f, #e4c10c)'
    },
    {
      name: 'Tailwind CSS',
      level: 85,
      icon: '🎨',
      description: 'Crafting responsive UI with Tailwind CSS.',
      cardGradient: 'linear-gradient(to right, #38b2ac, #4fd1c5)',
      barGradient: 'linear-gradient(to right, #38b2ac, #06b6d4)'
    },
    {
      name: 'Django',
      level: 80,
      icon: '🍃',
      description: 'Backend web development with Django & DRF.',
      cardGradient: 'linear-gradient(to right, #0c4b33, #0a3d2f)',
      barGradient: 'linear-gradient(to right, #0c4b33, #16a34a)'
    },
    {
      name: 'Flutter',
      level: 75,
      icon: '📱',
      description: 'Cross-platform apps for iOS & Android.',
      cardGradient: 'linear-gradient(to right, #02569b, #00bcd4)',
      barGradient: 'linear-gradient(to right, #02569b, #06b6d4)'
    },
    {
      name: 'Python',
      level: 88,
      icon: '🐍',
      description: 'Data processing, scripting, and backend development.',
      cardGradient: 'linear-gradient(to right, #306998, #FFD43B)',
      barGradient: 'linear-gradient(to right, #306998, #facc15)'
    },
    {
      name: 'HTML5',
      level: 95,
      icon: '📄',
      description: 'Semantic HTML structure for web pages.',
      cardGradient: 'linear-gradient(to right, #e44d26, #f16529)',
      barGradient: 'linear-gradient(to right, #e44d26, #f97316)'
    },
    {
      name: 'CSS3',
      level: 90,
      icon: '🎨',
      description: 'Modern CSS techniques including Flex & Grid.',
      cardGradient: 'linear-gradient(to right, #2965f1, #1e40af)',
      barGradient: 'linear-gradient(to right, #2965f1, #3b82f6)'
    },
    {
      name: 'Git & GitHub',
      level: 85,
      icon: '🔧',
      description: 'Version control and collaboration workflow.',
      cardGradient: 'linear-gradient(to right, #f05032, #181717)',
      barGradient: 'linear-gradient(to right, #f05032, #f97316)'
    },
  ]
  </script>
  
  <style scoped>
  .skills-section {
    padding: 6rem 2rem;
    margin-top: 6rem;        /* space above section */
    margin-bottom: 6rem;   /* space below section */
    /* width: 100%; */
    background: #1a202c; /* dark background */
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
  
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2.5rem;
  }
  
  .skill-card {
    padding: 2rem;
    border-radius: 2rem;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
    transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
  }
  
  .skill-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.5);
  }
  
  .skill-header {
    display: flex;
    align-items: center;
    margin-bottom: 1rem;
  }
  
  .skill-icon {
    font-size: 2rem;
    margin-right: 1rem;
  }
  
  .skill-name {
    font-size: 1.5rem;
    font-weight: bold;
  }
  
  .progress-bar {
    width: 100%;
    height: 1.5rem;
    background: #2d3748; /* dark gray */
    border-radius: 1rem;
    overflow: hidden;
    margin: 0.5rem 0;
  }
  
  .progress-fill {
    height: 100%;
    border-radius: 1rem;
    transition: width 1s ease-in-out;
  }
  
  .skill-level {
    font-weight: 600;
    margin-top: 0.5rem;
  }
  
  .skill-desc {
    font-size: 0.875rem;
    color: #e2e8f0; /* light gray text */
    margin-top: 0.25rem;
  }
  </style>
  