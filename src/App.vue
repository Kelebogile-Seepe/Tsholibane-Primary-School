<template>
  <div id="app">
    <!-- Navbar -->
    <HelloWorld />

    <!-- Sections -->
    <section id="home">
      <HomePage />
    </section>

    <section id="about">
      <AboutPage />
    </section>

    <section id="projects">
      <ProjectsSection />
    </section>

    <section id="contact">
      <ContactMe />
    </section>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomePage from './components/HomePage.vue'
import AboutPage from './components/AboutPage.vue'
import ProjectsSection from './components/ProjectsSection.vue'
import ContactMe from './components/ContactMe.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    HomePage,
    AboutPage,
    ProjectsSection,
    ContactMe
  }
}
</script>
<style scoped>
.nav-links li a:hover {
  color: #38bdf8; 
}
</style>