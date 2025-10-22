<template>
  <div>

    <nav class="navbar">
      <div class="hamburger" @click="toggleMenu">
        <i class="pi pi-bars"></i>
      </div>

      <ul :class="['nav-links', { show: menuOpen }]">
        <li><a href="#home" @click="closeMenu"><i class="pi pi-home"></i> Home</a></li>
        <li><a href="#about" @click="closeMenu"><i class="pi pi-user"></i> Activities</a></li>
        <!--<li><a href="#services" @click="closeMenu"><i class="pi pi-cog"></i> Services</a></li>-->
        <li><a href="#projects" @click="closeMenu"><i class="pi pi-folder"></i> Staff Profile</a></li>
        <li><a href="#contact" @click="closeMenu"><i class="pi pi-phone"></i> Contact Us</a></li>
      </ul>
    </nav>
  </div>
</template>


<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      menuOpen: false
    }
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen
    },
    closeMenu() {
      this.menuOpen = false
    }
  }
 
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background:White;
  color:  #c0392b;
  padding: 1rem;
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 1000;
}

.logo {
  font-size: 1.5rem;
}

.hamburger {
  display: none;
  font-size: 2rem;
  cursor: pointer;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.nav-links li a {
  text-decoration: none;
  color: #c0392b;
  transition: color 0.3s;
}

.nav-links li a:hover {
  color:  #c2b968;
}

@media (max-width: 768px) {
  .hamburger {
    display: block;
  }

  .nav-links {
    display: none;
    flex-direction: column;
    background:white;
    position: absolute;
    top: 60px;
    left: 0;
    width: 100%;
    padding: 1rem 0;

  }

  .nav-links.show {
    display: flex;
  }

  .nav-links li {
    text-align: center;
    margin: 10px 0;
  }
}
</style>
