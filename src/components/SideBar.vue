<template>
    <aside class="sidebar">
      <div class="sidebar-inner">
        <div class="profile">
          <!-- <img :src="require('@/assets/profile.jpg')" alt="Profile" /> -->
        </div>
  
        <nav class="nav-links">
          <a href="#hero">
            <span class="icon">🏠</span> Home
          </a>
          <a href="#about">
            <span class="icon">👨‍💻</span> About
          </a>
          <a href="#skills">
            <span class="icon">💡</span> Skills
          </a>
          <a href="#projects">
            <span class="icon">📁</span> Projects
          </a>
          <a href="#contact">
            <span class="icon">✉️</span> Contact
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
  /* Sidebar container */
    .sidebar {
    position: fixed;
    top: 50%;
    left: 15px;
    transform: translateY(-50%);
    width: 220px;
    height: 800px;
    background: #111827;
    border-radius: 1rem; /* all corners curved equally */
    border: 2px solid #fff; /* white border */
    box-shadow: 2px 0 15px rgba(0, 0, 0, 0.5);
    z-index: 50;
    padding: 2rem 0;
    transition: border-color 0.3s ease, transform 0.3s ease;
    }

    /* Optional: border color on hover */
    .sidebar:hover {
    border-color: #10b981; /* green on hover */
    }


  
  /* Inner container */
  .sidebar-inner {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
  }
  
  /* Profile image */
  .profile img {
    width: 60px;
    height: 60px;
    border-radius: 9999px;
    border: 2px solid white;
    object-fit: cover;
    margin-bottom: 1rem;
  }
  
  /* Navigation links */
  .nav-links {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
    width: 100%;
  }
  
  /* Link styles with full border */
  .nav-links a {
    display: flex;
    align-items: center;
    gap: 0.75rem;
    padding: 0.5rem 1rem;
    color: #fff;
    font-size: 1.2rem;
    text-decoration: none;
    border: 2px solid #fff; /* white border for entire link */
    border-radius: 0.75rem;
    transition: all 0.3s ease;
  }
  
  /* Hover effect for whole link */
  .nav-links a:hover {
    color: #10b981; /* text color green */
    border-color: #10b981; /* border color green */
    transform: scale(1.1);
  }
  
  /* Icon inside link */
  .nav-links .icon {
    font-size: 1.3rem;
  }
  
  /* Smooth scrolling */
  html {
    scroll-behavior: smooth;
  }
  </style>
  