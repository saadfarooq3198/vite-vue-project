<script setup>
import "./components/blogComponent.vue";
import blogComponent from "./components/blogComponent.vue";
import eventComponent from "./components/eventComponent.vue";
import { blogs } from "./data/blogs";
import { speaking } from "./data/events";
</script>

<template>
  <section class="hero">
    <header class="navbar">
      <nav class="links">
        <a href="#">Blog</a>
        <a href="#">Speaking Events</a>
      </nav>
      <p>Hazel</p>
      <a class="contact" href="#contact">Contact Me</a>
    </header>
    <div class="hero-content">
      <h1 class="tagline">
        I'm a <em>Scientist</em> and <em>Speaker</em> who is interested in the
        psychology of greed.
      </h1>
      <div class="two-column-section">
        <p>My Mission</p>
        <p>
          This is my mission. Maecenas a varius odio egestas auctor. Praesent
          facilisis, ex a gravida ultricies, quam sed megna placerat eros, et
          vehicula lectus ligula id dui. Aliquam uto cursus velit ut eros lorem
          ispum ullamcorper iaculis.
        </p>
      </div>
      <div class="two-column-section">
        <p>Specialties</p>
        <ul class="skills">
          <li>Public Speaking</li>
          <li>Data Analysis</li>
          <li>Data Analysis</li>
          <li>User Interviews</li>
          <li>Writing & Editing</li>
          <li>Analytics & Data</li>
          <li>Front-End Dev</li>
          <li>Programming</li>
        </ul>
      </div>
    </div>
  </section>
  <blogComponent :blogs="blogs" />

  <eventComponent :speaking="speaking" />

 

  <footer>
    <div class="footer-content">
      <img src="./assets/instagram.png" alt="instagran" />
      <img src="./assets/twitter.png" alt="twitter" />
      <p>Made with ❤️</p>
    </div>
  </footer>
</template>


<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
