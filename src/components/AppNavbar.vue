<template>
  <nav class="navbar">
    <ul>
      <li><a href="#hero">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "AppNavbar",
};
</script>

<style scoped>
.navbar {
  background: #2c3e50;
  padding: 1rem;
}
.navbar ul {
  list-style: none;
  display: flex;
  justify-content: center;
}
.navbar li {
  margin: 0 15px;
}
.navbar a {
  color: white;
  text-decoration: none;
}
</style>
