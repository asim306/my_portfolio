<template>
  <section id="hero" class="hero">
    <h1>Hi, I'm Asim Mahmood </h1>
    <p>A Web & Mobile App Developer</p>
  </section>
</template>

<script>
export default {
  name: "HeroBanner",
};
</script>

<style scoped>
.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: linear-gradient(to right, #00c6ff, #0072ff);
  color: white;
  text-align: center;
}
</style>
