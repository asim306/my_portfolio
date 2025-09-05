<template>
  <section id="contact" class="contact-section">
    <div class="container">
      <!-- Section Title -->
      <div class="section-title">
        <h2>Contact</h2>
        <p>Necessitatibus eius consequatur ex aliquid fuga eum quidem sint consectetur velit</p>
      </div>

      <!-- Contact Content -->
      <div class="contact-content">
        <!-- Left: Contact Info -->
        <div class="contact-info">
          <h3>Contact Info</h3>
          <p>
            Praesent sapien massa, convallis a pellentesque nec, egestas non nisi.
            Vestibulum ante ipsum primis.
          </p>

          <div class="info-item">
            <i class="fas fa-map-marker-alt"></i>
            <div>
              <h4>Our Location</h4>
              <p>A108 Adam Street <br> New York, NY 535022</p>
            </div>
          </div>

          <div class="info-item">
            <i class="fas fa-phone"></i>
            <div>
              <h4>Phone Number</h4>
              <p>+1 5589 55488 55 <br> +1 6678 254445 41</p>
            </div>
          </div>

          <div class="info-item">
            <i class="fas fa-envelope"></i>
            <div>
              <h4>Email Address</h4>
              <p>info@example.com <br> contact@example.com</p>
            </div>
          </div>
        </div>

        <!-- Right: Contact Form -->
        <div class="contact-form">
          <h3>Get In Touch</h3>
          <p>
            Praesent sapien massa, convallis a pellentesque nec, egestas non nisi.
            Vestibulum ante ipsum primis.
          </p>

          <form>
            <div class="form-row">
              <input type="text" placeholder="Your Name" required>
              <input type="email" placeholder="Your Email" required>
            </div>
            <input type="text" placeholder="Subject" required>
            <textarea rows="5" placeholder="Message" required></textarea>
            <button type="submit">Send Message</button>
          </form>
        </div>
      </div>
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
  padding: 6rem 2rem;
  background: #111; /* Dark background */
  color: #fff;
}

.section-title {
  text-align: center;
  margin-bottom: 3rem;
}

.section-title h2 {
  font-size: 2rem;
  font-weight: bold;
  position: relative;
  display: inline-block;
  margin-bottom: 0.5rem;
}

.contact-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
}

/* Left Card */
.contact-info {
  background: #f9f9f9;
  color: #333;
  padding: 2rem;
  border-radius: 1rem;
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.contact-info h3 {
  margin-bottom: 1rem;
  font-size: 1.5rem;
  color: #6a1b1b;
}

.info-item {
  display: flex;
  align-items: center;
  margin-top: 1.5rem;
}

.info-item i {
  font-size: 1.5rem;
  margin-right: 1rem;
  color: #6a1b1b;
  background: #eee;
  padding: 1rem;
  border-radius: 50%;
}

/* Right Card */
.contact-form {
  background: #1a1a1a;
  padding: 2rem;
  border-radius: 1rem;
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.contact-form h3 {
  margin-bottom: 1rem;
  font-size: 1.5rem;
}

.contact-form form {
  display: flex;
  flex-direction: column;
}

.form-row {
  display: flex;
  gap: 1rem;
  margin-bottom: 1rem;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 0.75rem;
  margin-bottom: 1rem;
  border: none;
  border-radius: 0.5rem;
  background: #2c2c2c;
  color: #fff;
}

.contact-form input::placeholder,
.contact-form textarea::placeholder {
  color: #aaa;
}

.contact-form button {
  align-self: flex-start;
  background: #fff;
  color: #6a1b1b;
  padding: 0.75rem 2rem;
  border: none;
  border-radius: 2rem;
  font-weight: bold;
  cursor: pointer;
  transition: 0.3s;
}

.contact-form button:hover {
  background: #6a1b1b;
  color: #fff;
}
</style>
