<template>
  <section class="activities-section" id="activities">
    <div class="header">
      <h1>Exciting School Activities</h1>
      <p>
        Discover the vibrant life at our primary school with a variety of engaging events
        and memorable experiences for every student.
      </p>
    </div>

    <div class="activities-grid">
      <div class="activity-card">
        <img src="../assets/market.webp" alt="Annual Market Day" />
        <div class="card-content">
          <h3>Annual Market Day</h3>
          <p>
            A lively event where students showcase their entrepreneurial skills, selling
            handmade crafts and delicious treats. A fantastic opportunity for learning and
            community bonding.
          </p>
          <button>Learn More</button>
        </div>
      </div>

      <div class="activity-card">
        <img src="../assets/funday.webp" alt="Summer Fun Day" />
        <div class="card-content">
          <h3>Summer Fun Day</h3>
          <p>
            An exciting day filled with games, sports, and entertainment for all students.
            We celebrate achievements and friendships, creating lasting memories for
            everyone.
          </p>
          <button>Learn More</button>
        </div>
      </div>

      <div class="activity-card">
        <img src="../assets/heritage.webp" alt="Heritage Day Celebration" />
        <div class="card-content">
          <h3>Heritage Day Celebration</h3>
          <p>
            Students explore and celebrate the diverse cultures and traditions that make
            up our school community through performances, food, and art.
          </p>
          <button>Learn More</button>
        </div>
      </div>

      <div class="activity-card">
        <img src="../assets/farewell.webp" alt="Grade 7 Farewell Day" />
        <div class="card-content">
          <h3>Grade 7 Farewell Day</h3>
          <p>
            A memorable day dedicated to our graduating Grade 7s, honoring their journey
            and achievements with a special ceremony and celebration.
          </p>
          <button>Learn More</button>
        </div>
      </div>

      <div class="activity-card">
        <img src="../assets/science.webp" alt="Annual Science Fair" />
        <div class="card-content">
          <h3>Annual Science Fair</h3>
          <p>
            Young scientists present their innovative projects, fostering curiosity and a
            love for discovery. An inspiring event for all ages.
          </p>
          <button>Learn More</button>
        </div>
      </div>

      <div class="activity-card">
        <img src="../assets/drama.webp" alt="School Drama Production" />
        <div class="card-content">
          <h3>School Drama Production</h3>
          <p>
            Our talented students showcase their acting and stage skills in an annual
            drama production, bringing stories to life.
          </p>
          <button>Learn More</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ActivitiesSection",
};
</script>

<style scoped>
.activities-section {
  font-family: "Segoe UI", sans-serif;
  padding: 4rem 2rem;
  background-color: #fff;
  text-align: center;
}

/* === Header === */
.header {
  max-width: 800px;
  margin: 0 auto 3rem;
}

.header h1 {
  font-size: 2.2rem;
  font-weight: 700;
  color: #222;
  margin-bottom: 1rem;
}

.header p {
  color: #555;
  font-size: 1.1rem;
  line-height: 1.6;
}

/* === Activities Grid === */
.activities-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  max-width: 1100px;
  margin: 0 auto;
}

/* === Activity Card === */
.activity-card {
  background: #fff;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
  display: flex;
  flex-direction: column;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.activity-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
}

.activity-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.card-content {
  padding: 1.5rem;
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.card-content h3 {
  font-size: 1.3rem;
  color: #222;
  margin-bottom: 0.8rem;
}

.card-content p {
  color: #555;
  font-size: 0.95rem;
  line-height: 1.5;
  margin-bottom: 1.2rem;
}

button {
  background-color: #c0392b;
  color: white;
  border: none;
  padding: 0.7rem 1.4rem;
  border-radius: 25px;
  font-weight: bold;
  cursor: pointer;
  align-self: center;
  transition: background 0.3s ease;
}

button:hover {
  background-color: #a93226;
}

/* === Responsive Design === */
@media (max-width: 900px) {
  .header h1 {
    font-size: 2rem;
  }
  .header p {
    font-size: 1rem;
  }
}

@media (max-width: 600px) {
  .activities-section {
    padding: 3rem 1rem;
  }
  .header h1 {
    font-size: 1.8rem;
  }
  .activity-card img {
    height: 180px;
  }
  button {
    padding: 0.6rem 1.2rem;
  }
}
</style>
