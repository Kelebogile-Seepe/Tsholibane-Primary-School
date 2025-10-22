<template>
  <div class="harmony-page">
    <section class="hero">
      <div class="hero-content">
        <div class="hero-text">
          <h1>Tsokolibane Primary School</h1>
          <p class="subtitle">Nurturing Young Minds, Building Bright Futures</p>
          <p class="desc">
            At Tsokolibane Primary School, we believe in fostering a love for learning through creativity, curiosity, and collaboration. We strive to empower every child to reach their full potential in a nurturing and inclusive environment.
          </p>
          <button class="hero-btn">Learn More</button>
        </div>
        <div class="hero-image">
          <img src="../assets/image (1).png" alt="Students" />
        </div>
      </div>
    </section>

    <!-- Welcome Section -->
    <section class="welcome">
      <h2>Welcome to Tsokolibane Primary School</h2>
      <p>
        Tsokolibane Primary School is a beacon of elementary education committed to providing a holistic learning experience. Our dedicated educators inspire curiosity, creativity, and critical thinking, ensuring our learners become confident and responsible global citizens.
      </p>
    </section>

    <!-- Legacy Section -->
    <section class="legacy">
      <div class="legacy-content">
        <div class="legacy-image">
          <img src="../assets/kele.jpg" alt="School Building" />
        </div>
        <div class="legacy-text">
          <h3>Our Legacy: A Foundation of Excellence</h3>
          <ul>
            <li><strong>Established in 1978:</strong> With a clear mission to provide quality education for all learners.</li>
            <li><strong>Dedication:</strong> Tsokolibaney Primary has a tradition of fostering growth and excellence for generations.</li>
            <li><strong>Commitment:</strong> We prepare our students for the bigger world through a blend of traditional and modern learning approaches.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Guiding Principles -->
    <section class="principles">
      <h3>Our Guiding Principles</h3>
      <div class="principle-cards">
        <div class="card">
          <h4>Our Vision</h4>
          <p>
            To cultivate an environment that harnesses curiosity and creativity — helping learners develop a lifelong passion for learning.
          </p>
        </div>
        <div class="card">
          <h4>Our Mission</h4>
          <p>
            We embrace excellence, collaboration, and self-discipline — ensuring every child is empowered with the skills and confidence to succeed.
          </p>
        </div>
      </div>
    </section>

    <!-- Why Choose Section -->
    <section class="why-choose">
      <h3>Why Choose Tsokolibane Primary?</h3>
      <div class="choose-grid">
        <div class="choose-card">
          <h5>Academic Excellence</h5>
          <p>High academic standards with individualized learning support for every child.</p>
        </div>
        <div class="choose-card">
          <h5>Holistic Development</h5>
          <p>Balanced programs focusing on academics, arts, sports, and emotional growth.</p>
        </div>
        <div class="choose-card">
          <h5>Vibrant Community</h5>
          <p>A warm, inclusive environment where diversity and collaboration thrive.</p>
        </div>
        <div class="choose-card">
          <h5>Innovative Approach</h5>
          <p>Modern teaching methods designed to engage, inspire, and empower learners.</p>
        </div>
        <div class="choose-card">
          <h5>Strong Partnerships</h5>
          <p>We value collaboration among teachers, parents, and the broader community.</p>
        </div>
        <div class="choose-card">
          <h5>Rich Extracurriculars</h5>
          <p>Clubs, arts, and sports programs that help learners discover their passions.</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "HomePage",
};
</script>

<style scoped>
/* === Global Styles === */
.harmony-page {
  font-family: "Segoe UI", sans-serif;
  color: #333;
  line-height: 1.6;
}

/* === Hero Section === */
.hero {
  background-color: #fdecec;
  padding: 4rem 2rem;
}

.hero-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  max-width: 1100px;
  margin: auto;
}

.hero-text {
  flex: 1 1 45%;
}

.hero-text h1 {
  font-size: 2.8rem;
  font-weight: 700;
  color: #333;
}

.subtitle {
  color: #9b59b6;
  font-size: 1.2rem;
  margin: 0.8rem 0;
}

.desc {
  color: #555;
  margin-bottom: 1.5rem;
}

.hero-btn {
  background-color: #c0392b;
  color: #fff;
  border: none;
  padding: 0.8rem 1.6rem;
  border-radius: 8px;
  cursor: pointer;
  font-weight: bold;
  transition: background 0.3s ease;
}

.hero-btn:hover {
  background-color: #a93226;
}

.hero-image {
  flex: 1 1 45%;
  text-align: center;
}

.hero-image img {
  width: 100%;
  max-width: 400px;
  border-radius: 12px;
}

/* === Welcome Section === */
.welcome {
  text-align: center;
  max-width: 900px;
  margin: 3rem auto;
  padding: 0 1rem;
}

.welcome h2 {
  font-size: 2rem;
  margin-bottom: 1rem;
  color: #222;
}

/* === Legacy Section === */
.legacy {
  background-color: #fafafa;
  padding: 3rem 2rem;
}

.legacy-content {
  display: flex;
  flex-wrap: wrap;
  max-width: 1000px;
  margin: auto;
  align-items: center;
  gap: 2rem;
}

.legacy-image {
  flex: 1 1 45%;
  text-align: center;
}

.legacy-image img {
  width: 100%;
  max-width: 400px;
  border-radius: 10px;
}

.legacy-text {
  flex: 1 1 50%;
}

.legacy-text h3 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.legacy-text ul {
  list-style: disc;
  padding-left: 1.5rem;
}

/* === Guiding Principles === */
.principles {
  text-align: center;
  padding: 3rem 2rem;
}

.principle-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
  margin-top: 2rem;
}

.card {
  background: #fff;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  padding: 2rem;
  flex: 1 1 300px;
  max-width: 400px;
}

.card h4 {
  color: #9b59b6;
  margin-bottom: 1rem;
}

/* === Why Choose Section === */
.why-choose {
  background-color: #fafafa;
  text-align: center;
  padding: 3rem 2rem;
}

.choose-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  max-width: 1000px;
  margin: 2rem auto 0;
}

.choose-card {
  background: #fff;
  border-radius: 10px;
  padding: 1.5rem;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

.choose-card h5 {
  color: #c0392b;
  margin-bottom: 0.8rem;
}

/* === Responsive === */
@media (max-width: 1024px) {
  .hero-content {
    flex-direction: column;
    text-align: center;
  }

  .hero-text {
    margin-bottom: 2rem;
  }

  .legacy-content {
    flex-direction: column;
  }

  .legacy-text {
    text-align: center;
  }
}

@media (max-width: 600px) {
  .hero-text h1 {
    font-size: 2rem;
  }

  .hero-btn {
    padding: 0.7rem 1.4rem;
  }

  .card {
    padding: 1.5rem;
  }
}
</style>
