<template>
  <section class="staff-section">
    <!-- Leadership -->
    <div class="section leadership">
      <h2>Meet Our Leadership</h2>
      <div class="leader-card">
        <img src="@/assets/kele.jpg" alt="Dr. Eleanor Vance" />
        <h3>Dr. Eleanor Vance</h3>
        <p>Principal</p>
      </div>
    </div>

    <!-- Educators -->
    <div class="section educators">
      <h2>Our Dedicated Educators</h2>
      <div class="card-grid">
        <div v-for="(teacher, index) in teachers" :key="index" class="profile-card">
          <img :src="teacher.image" :alt="teacher.name" />
          <h3>{{ teacher.name }}</h3>
          <p>{{ teacher.title }}</p>
        </div>
      </div>
    </div>

    <!-- SGB Members -->
    <div class="section sgb">
      <h2>School Governing Body (SGB) Members</h2>
      <div class="card-grid">
        <div v-for="(member, index) in sgbMembers" :key="index" class="profile-card">
          <img :src="member.image" :alt="member.name" />
          <h3>{{ member.name }}</h3>
          <p>{{ member.role }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "StaffSection",
  data() {
  return {
    teachers: [
      { name: "Ms. Sarah Chen", title: "Grade 1 Teacher", image: require('@/assets/kele.jpg') },
      { name: "Mr. David Miller", title: "Grade 2 Teacher", image: require('@/assets/kele.jpg') },
      { name: "Mrs. Emily White", title: "Grade 3 Teacher", image: require('@/assets/kele.jpg') },
      { name: "Mr. James Brown", title: "Grade 4 Teacher", image: require('@/assets/kele.jpg') },
      { name: "Ms. Jessica Lee", title: "Grade 5 Teacher", image: require('@/assets/kele.jpg') },
      { name: "Mr. Robert Green", title: "Grade 6 Teacher", image: require('@/assets/kele.jpg') },
    ],
    sgbMembers: [
      { name: "Mr. Alex Johnson", role: "SGB Chairperson", image: require('@/assets/kele.jpg') },
      { name: "Mrs. Linda Davis", role: "SGB Secretary", image: require('@/assets/kele.jpg') },
      { name: "Mr. Kevin Wilson", role: "Parent Representative", image: require('@/assets/kele.jpg') },
      { name: "Ms. Olivia Martinez", role: "Parent Representative", image: require('@/assets/kele.jpg') },
      { name: "Dr. Marcus Reed", role: "Community Representative", image: require('@/assets/kele.jpg') },
      { name: "Ms. Chloe Taylor", role: "Educator Representative", image: require('@/assets/kele.jpg') },
    ],
  };
}

};
</script>

<style scoped>
.staff-section {
  font-family: 'Segoe UI', sans-serif;
  background-color: #fff;
  color: #333;
  padding: 60px 20px;
}

.section {
  text-align: center;
  margin-bottom: 60px;
}

.section h2 {
  color: #e53935;
  margin-bottom: 40px;
  font-size: 1.8rem;
}

.leadership {
  background-color: #fff5f5;
  padding: 40px 20px;
  border-radius: 10px;
}

.leader-card {
  display: inline-block;
  background-color: white;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.leader-card:hover {
  transform: translateY(-5px);
}

.leader-card img {
  width: 120px;
  height: 120px;
  object-fit: cover;
  border-radius: 50%;
  margin-bottom: 15px;
}

.card-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 25px;
}

.profile-card {
  background-color: #fff;
  border-radius: 12px;
  padding: 20px;
  width: 180px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  text-align: center;
  transition: transform 0.3s ease;
}

.profile-card:hover {
  transform: translateY(-6px);
}

.profile-card img {
  width: 100px;
  height: 100px;
  object-fit: cover;
  border-radius: 50%;
  margin-bottom: 12px;
}

.profile-card h3 {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 6px;
}

.profile-card p {
  font-size: 0.9rem;
  color: #555;
}

/* Responsive layout */
@media (max-width: 900px) {
  .profile-card {
    width: 160px;
  }
}

@media (max-width: 600px) {
  .card-grid {
    flex-direction: column;
    align-items: center;
  }
  .profile-card {
    width: 80%;
    max-width: 280px;
  }
}
</style>
