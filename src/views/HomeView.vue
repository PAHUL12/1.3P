<template>
  <section class="home-view">
      <div class="content-container">
          <h2>Welcome to My Portfolio</h2>
          <p>Welcome to my portfolio homepage.</p>
          <router-link to="/about" class="about-link">Learn more about me</router-link>
      </div>
  </section>
</template>

<script>
export default {
  name: 'HomeComponent',  /* Renamed to a more general 'HomeComponent' */
};
</script>

<style scoped>
.home-view {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: linear-gradient(135deg, #6B73FF, #000DFF);
  color: #f5f5f5;
  font-family: 'Arial', sans-serif;
  text-align: center;
  overflow: hidden; /* To avoid any scroll issues */
  position: relative;
}

.content-container {
  z-index: 1; /* Ensure content is above any potential background elements */
}

.home-view h2 {
  font-size: 2.7rem; /* Slightly increased for emphasis */
  margin-bottom: 25px; /* Increased spacing for better separation */
  text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.2);
}

.home-view p {
  font-size: 1.3rem; /* Increased for readability */
  margin-bottom: 25px; /* Increased spacing for better separation */
}

.about-link {
  background-color: #F5F5F5;
  color: #333;
  padding: 12px 25px; /* Increased padding for better touch target */
  border-radius: 7px; /* Slightly larger radius */
  text-decoration: none;
  font-weight: bold;
  transition: background-color 0.2s, transform 0.2s; /* Added transform for hover effect */
}

.about-link:hover {
  background-color: #DDD;
  transform: scale(1.05); /* Slight scaling for interactive feedback */
}
</style>
