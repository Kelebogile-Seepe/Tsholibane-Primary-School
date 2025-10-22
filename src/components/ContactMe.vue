<template>
  <section class="contact-section" id="contact">
    <div class="contact-container">
      <h1 class="contact-title">Get In Touch With Me</h1>

      <div class="contact-grid">
        <!-- Left: Contact Info -->
        <div class="contact-info">
          <div class="info-card">
            <i class="pi pi-map-marker info-icon"></i>
            <div>
              <h3>My Address</h3>
              <p>Johannesburg, South Africa</p>
              <a href="https://maps.google.com" target="_blank">View on Map</a>
            </div>
          </div>

          <div class="info-card">
            <i class="pi pi-phone info-icon"></i>
            <div>
              <h3>Call Me</h3>
              <p>+27 82 066 9203</p>
              <a href="tel:+27820669203">Dial Now</a>
            </div>
          </div>

          <div class="info-card">
            <i class="pi pi-envelope info-icon"></i>
            <div>
              <h3>Email Me</h3>
              <p>kelebogileseepe@gmail.com</p>
              <a href="mailto:kelebogileseepe@gmail.com">Send Email</a>
            </div>
          </div>

          <div class="info-card">
            <i class="pi pi-linkedin info-icon"></i>
            <div>
              <h3>LinkedIn</h3>
              <p>Kelebogile Seepe</p>
              <a href="https://www.linkedin.com/in/kelebogile-seepe-3300bb257/" target="_blank">
                View Profile
              </a>
            </div>
          </div>

          <div class="info-card">
            <i class="pi pi-file-pdf info-icon"></i>
            <div>
              <h3>My CV</h3>
              <p>Download my latest CV</p>
              <a href="/Kelebogile.pdf" download>Download</a>
            </div>
          </div>
        </div>

        <!-- Right: Contact Form -->
        <div class="contact-form">
          <h3>Send Me a Message</h3>
          <form @submit.prevent="sendMessage">
            <label>Your Name</label>
            <input type="text" placeholder="John Doe" v-model="form.name" required />

            <label>Your Email</label>
            <input type="email" placeholder="john.doe@example.com" v-model="form.email" required />

            <label>Subject</label>
            <input type="text" placeholder="Inquiry about collaboration" v-model="form.subject" />

            <label>Your Message</label>
            <textarea rows="4" placeholder="Type your message here..." v-model="form.message"></textarea>

            <button type="submit" class="send-btn">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import "primeicons/primeicons.css";

export default {
  name: "ContactMe",
  data() {
    return {
      form: {
        name: "",
        email: "",
        subject: "",
        message: "",
      },
    };
  },
  methods: {
    sendMessage() {
      alert("Message sent successfully!");
      this.form = { name: "", email: "", subject: "", message: "" };
    },
  },
};
</script>

<style scoped>
.contact-section {
  background-color: #f9fafb;
  padding: 80px 20px;
  font-family: "Segoe UI", sans-serif;
}

.contact-container {
  max-width: 1100px;
  margin: auto;
}

.contact-title {
  text-align: center;
  font-size: 2.2rem;
  font-weight: bold;
  color: #111827;
  margin-bottom: 40px;
}

.contact-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
}

.contact-info,
.contact-form {
  background: white;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  padding: 30px;
  flex: 1;
  min-width: 300px;
}

.contact-info {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.info-card {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
}

.info-icon {
  color: #ef4444;
  font-size: 1.6rem;
  margin-top: 5px;
}

.info-card h3 {
  margin: 0;
  font-size: 1.1rem;
  color: #111827;
}

.info-card p {
  margin: 2px 0;
  color: #374151;
}

.info-card a {
  color: #ef4444;
  text-decoration: none;
  font-weight: 500;
}

.info-card a:hover {
  text-decoration: underline;
}

.contact-form h3 {
  font-size: 1.4rem;
  margin-bottom: 1.5rem;
  color: #111827;
}

form {
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}

input,
textarea {
  padding: 10px;
  border: 1px solid #d1d5db;
  border-radius: 6px;
  font-size: 1rem;
}

input:focus,
textarea:focus {
  border-color: #ef4444;
  outline: none;
}

.send-btn {
  background-color: #ef4444;
  color: white;
  border: none;
  padding: 12px;
  border-radius: 6px;
  font-weight: 600;
  cursor: pointer;
  transition: 0.3s;
}

.send-btn:hover {
  background-color: #dc2626;
}

/* Responsive */
@media (max-width: 900px) {
  .contact-grid {
    flex-direction: column;
  }
}
</style>
