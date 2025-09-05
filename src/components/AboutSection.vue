<template>
  <section id="about" class="about-section">
    <div class="container">
      <!-- Left Card -->
      <div class="profile-card">
        <div class="profile-img">
          <img src="@/assets/logo.png" alt="Profile" />
        </div>
        <h2>Qasim Mahmood</h2>
        <p class="role">Web & Mobile Developer</p>

       <!-- Contact Info -->
       <div class="contact-info">
        <a href="mailto:asimmahmood199@gmail.com" class="contact-item">
          asimmahmood199@gmail.com <i class="fas fa-envelope"></i>
        </a>
        <a href="tel:+923001234567" class="contact-item">
          +92 300 1234567 <i class="fas fa-phone"></i>
        </a>
        <a
          href="https://www.google.com/maps/place/Rawalpindi,+Pakistan"
          target="_blank"
          rel="noopener"
          class="contact-item"
        >
          Rawalpindi, Pakistan <i class="fas fa-map-marker-alt"></i>
        </a>
      </div>



      </div>

      <!-- Right Info -->
      <div class="about-content">
        <button class="intro-btn">Get to Know Me</button>
        <h2 class="title">Passionate About Creating Digital Experiences</h2>
        <p class="description">
          I’m a web & mobile developer passionate about clean code, innovative solutions,
          and creating beautiful, user-friendly interfaces. Experienced in Vue.js, Django,
          Flutter, and modern web technologies. I specialize in building responsive and scalable 
          web applications, intuitive mobile apps, and seamless user experiences.
        </p>
        <p class="description">
          I enjoy collaborating with teams to solve complex problems, optimize performance, 
          and deliver high-quality software. My expertise also includes API integration, 
          database design, and implementing best practices in front-end and back-end development.
        </p>

        <!-- Stats -->
        <div class="stats">
          <div class="stat"><h3>20+</h3><p>Projects Completed</p></div>
          <div class="stat"><h3>3+</h3><p>Years Experience</p></div>
          <div class="stat"><h3>95%</h3><p>Client Satisfaction</p></div>
        </div>

        <!-- Extra Info -->
        <div class="extra-info">
          <div><span>Specialization</span> UI/UX Design & Development</div>
          <div><span>Experience Level</span> Mid-Level Developer</div>
          <div><span>Education</span> Computer Science, COMSATS</div>
          <div><span>Languages</span> English, Urdu</div>
        </div>

        <!-- Buttons -->
        <div class="buttons">
          <a href="/resume.pdf" class="btn primary">⬇ Download Resume</a>
          <a href="#contact" class="btn secondary">💬 Let’s Talk</a>
        </div>
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
  padding: 6rem 2rem;
  background: #111; /* 0.5 = 50% transparent */
  display: flex;
  justify-content: center;
}

.container {
  max-width: 1200px;
  width: 100%;
  display: flex;
  gap: 2rem;
  flex-wrap: wrap;
}

/* Left profile card */
.profile-card {
  flex: 1;
  min-width: 280px;
  max-width: 350px;
  background: #1f1f1f;
  padding: 2rem;
  border-radius: 1.5rem;
  text-align: center;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
}
.profile-img img {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  border: 4px solid #fff;
  margin-bottom: 1rem;
}
.profile-card h2 {
  font-size: 1.5rem;
  margin-bottom: 0.25rem;
  font-weight: 700;
  color: #fff;
}
.profile-card .role {
  font-size: 0.95rem;
  color: #bbb;
  margin-bottom: 1.5rem;
}
.contact-info {
  text-align: left;
  font-size: 0.9rem;
  color: #ddd;
}
.contact-info div {
  margin: 0.5rem 0;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}
.contact-info i {
  color: #4ade80;
}

/* Right content */
.about-content {
  flex: 2;
  min-width: 350px;
  color: #fff;
}
.intro-btn {
  background: #fff;
  color: #111827;
  border: none;
  padding: 0.5rem 1.25rem;
  border-radius: 20px;
  font-weight: 600;
  margin-bottom: 1rem;
}
.title {
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 1rem;
}
.description {
  font-size: 1rem;
  color: #ccc;
  line-height: 1.6;
  margin-bottom: 1rem;
}

/* Stats */
.stats {
  display: flex;
  gap: 2rem;
  margin: 2rem 0;
  background: #1c1c1c;
  padding: 1rem;
  border-radius: 1rem;
}
.stat {
  text-align: center;
  flex: 1;
}
.stat h3 {
  font-size: 1.5rem;
  color: #4ade80;
}
.stat p {
  font-size: 0.9rem;
  color: #bbb;
}

/* Extra Info */
.extra-info {
  margin: 2rem 0;
}
.extra-info div {
  margin-bottom: 0.5rem;
}
.extra-info span {
  font-weight: bold;
  color: #bbb;
  margin-right: 0.5rem;
}

/* Buttons */
.buttons {
  display: flex;
  gap: 1rem;
}
.btn {
  padding: 0.75rem 1.25rem;
  border-radius: 8px;
  font-weight: 600;
  text-decoration: none;
  display: inline-block;
}
.btn.primary {
  background: #fff;
  color: #111827;
}
.btn.secondary {
  background: transparent;
  color: #fff;
  border: 1px solid #fff;
}

.contact-info {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 100%;
}

.contact-item {
  display: flex;
  justify-content: space-between; /* pushes icon to right */
  align-items: center;
  padding: 0.8rem 1rem;
  border: 2px solid #444; /* separate border for each item */
  border-radius: 10px;
  color: #ddd;
  text-decoration: none;
  font-size: 1rem;
  transition: all 0.3s ease;
}

.contact-item i {
  font-size: 1.2rem;
  color: #10b981; /* green for icons */
}

.contact-item:hover {
  background: rgba(255, 255, 255, 0.08);
  border-color: #10b981;
  color: #fff;
  transform: scale(1.03);
}

</style>
