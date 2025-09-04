<template>
  <section id="about" class="about-section">
    <div class="container">
      <div class="about-card">
        <h2>About Me</h2>
        <p>
          I’m a web & mobile developer passionate about clean code, innovative solutions, 
          and creating beautiful, user-friendly interfaces. Experienced in Vue.js, Django, 
          Flutter, and modern web technologies. I specialize in building responsive and scalable 
          web applications, intuitive mobile apps, and seamless user experiences. 

          I enjoy collaborating with teams to solve complex problems, optimize performance, 
          and deliver high-quality software. My expertise also includes API integration, 
          database design, and implementing best practices in front-end and back-end development. 

          Outside of coding, I am passionate about learning new technologies, contributing to 
          open-source projects, and exploring ways to make digital experiences more engaging 
          and accessible for everyone. My goal is to combine creativity with technical expertise 
          to build applications that delight users and solve real-world problems.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutSection",
};
</script>

<style scoped>
.about-section {
  padding: 6rem 2rem; /* full spacing above and below */
  margin-top: 6rem;   /* space above section */
  margin-bottom: 6rem; /* space below section */
  /* width: 100%; */
  background: linear-gradient(135deg, #1f2937, #111827); /* full-width background like others */
  display: flex;
  justify-content: center;
}

.container {
  max-width: 1200px;
  width: 100%;
  display: flex;
  justify-content: center;
}

.about-card {
  max-width: 800px;
  background-color: #1e40af; /* card color */
  color: white;
  padding: 3rem;
  border-radius: 2rem;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  text-align: center;
  transition: transform 0.3s ease-in-out;
}

.about-card:hover {
  transform: translateY(-8px);
}

.about-card h2 {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1.5rem;
}

.about-card p {
  font-size: 1.125rem;
  line-height: 1.75rem;
}
</style>
