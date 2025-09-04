<template>
  <section id="contact" class="contact-section">
    <div class="contact-card">
      <h2>Contact Me</h2>
      <p>Email: example@email.com</p>
      <p>Phone: +92 300 1234567</p>
      <p>Location: Rawalpindi, Pakistan</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactSection",
};
</script>

<style scoped>
.contact-section {
  padding: 6rem 2rem;      /* internal padding */
  margin-top: 6rem;        /* space above section */
  margin-bottom: 6rem;     /* space below section */
  background: #1f2937;     /* dark background matching portfolio */
  color: white;
  /* width: 100%; */
  text-align: center;
}

.contact-card {
  background: linear-gradient(135deg, #4f46e5, #6366f1);
  padding: 3rem;
  border-radius: 2rem;
  box-shadow: 0 10px 25px rgba(0,0,0,0.3);
}

.contact-card h2 {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1.5rem;
}

.contact-card p {
  font-size: 1.25rem;
  margin: 0.5rem 0;
}
</style>
