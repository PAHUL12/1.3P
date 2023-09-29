<template>
  <section class="about-view">
      <h2>About Me</h2>
      <p>
          My ambition is to find a position where my existing Customer Service talents & Tech enthusiasm could be applied in creating win-win situations for my employer and their customers. I take pride in my communication skills and problem-solving abilities in delivering value in my customer interactions.
      </p>
  </section>
</template>

<script>
export default {
  name: 'AboutComponent',  /* Renamed to a more general 'AboutComponent' */
};
</script>

<style scoped>
.about-view {
  text-align: left; /* Changed to left for more natural reading flow */
  padding: 40px 10%; /* Increased padding and added horizontal padding for better spacing */
  color: #E8E8E8; /* Slightly darker shade for better contrast */
  background-color: #333; /* Background color for the section */
  border-radius: 10px; /* Rounded corners */
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2); /* Subtle shadow for depth */
}

.about-view h2 {
  font-size: 2.5rem; /* Increased font size for better emphasis */
  margin-bottom: 30px; /* Increased spacing for better separation */
  border-bottom: 2px solid #555; /* Added a bottom border for stylistic separation */
  padding-bottom: 15px; /* Padding for the bottom border */
}
</style>
