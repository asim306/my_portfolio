<template>
  <aside class="sidebar">
    <div class="sidebar-inner">
      <div class="profile">
        <!-- <img :src="require('@/assets/profile.jpg')" alt="Profile" /> -->
      </div>

      <nav class="nav-links">
        <a href="#hero">
          <span class="icon">🏠</span> <span class="label">Home</span>
        </a>
        <a href="#about">
          <span class="icon">👨‍💻</span> <span class="label">About</span>
        </a>
        <a href="#skills">
          <span class="icon">💡</span> <span class="label">Skills</span>
        </a>
        <a href="#projects">
          <span class="icon">📁</span> <span class="label">Projects</span>
        </a>
        <a href="#contact">
          <span class="icon">✉️</span> <span class="label">Contact</span>
        </a>
      </nav>
    </div>
  </aside>
</template>

<script>
export default {
  name: 'SideBar',
}
</script>

<style scoped>
/* ========== Desktop Sidebar ========== */
.sidebar {
  position: fixed;
  top: 50%;
  left: 15px;
  transform: translateY(-50%);
  width: 250px;
  height: 800px;
  background: #111  ; /* 50% transparent */

  border-radius: 1rem;
  border: 2px solid #fff;
  box-shadow: 2px 0 15px rgba(0, 0, 0, 0.5);
  z-index: 50;
  padding: 2rem 0;
  transition: border-color 0.3s ease, transform 0.3s ease;
}

.sidebar:hover {
  border-color: #10b981;
}

.sidebar-inner {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.profile img {
  width: 60px;
  height: 60px;
  border-radius: 9999px;
  border: 2px solid white;
  object-fit: cover;
  margin-bottom: 1rem;
}

.nav-links {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  width: 100%;
}

.nav-links a {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  padding: 0.5rem 1rem;
  color: #fff;
  font-size: 1.2rem;
  text-decoration: none;
  /* border: 2px solid #fff; */
  border-radius: 0.75rem;
  transition: all 0.3s ease;
}

.nav-links a:hover {
  color: #10b981;
  border-color: #10b981;
  transform: scale(1.05);
}

.nav-links .icon {
  font-size: 1.3rem;
}

/* ========== Responsive (Tablet & Mobile) ========== */
@media (max-width: 1024px) {
  .sidebar {
    top: auto;
    bottom: 0;
    left: 0;
    width: 100%;
    height: auto;
    transform: none;
    border-radius: 1rem 1rem 0 0;
    display: flex;
    justify-content: center;
    padding: 0.75rem 1rem;
  }

  .sidebar-inner {
    flex-direction: row;
    justify-content: space-around;
    width: 100%;
    gap: 0;
  }

  .nav-links {
    flex-direction: row;
    gap: 0.5rem;
    width: 100%;
    justify-content: space-around;
  }

  .nav-links a {
    flex-direction: column;
    gap: 0.25rem;
    font-size: 0.9rem;
    border: none;
    background: transparent;
  }

  .nav-links a:hover {
    border: none;
    color: #10b981;
    transform: scale(1.1);
  }

  .label {
    font-size: 0.75rem;
  }
}
</style>
