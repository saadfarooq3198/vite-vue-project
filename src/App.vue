<script setup>
import HelloWorld from './components/HelloWorld.vue'

const blogs = [
  {
    'heading' : 'This Is Your Brain On Helium',
    'text' : "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolorum, voluptate mollitia voluptates iure harum autem facere aut cum. Dolorem, molestias animi nisi esse quam quo optio! Quidem nobis",
    'date' : 'May 19, 2025'
  },
  {
    'heading' : 'In Search Of Intelligence',
    'text' : "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolorum, voluptate mollitia voluptatesiure harum autem facere aut cum. Dolorem, molestias animi nisi esse quam quo optio! Quidem nobis inventore voluptatum.",
    'date' : 'June 12, 2025'
  },
  {
    'heading' : 'Should Public Transit Be Free?',
    'text' : "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolorum, voluptate mollitia voluptates iure harum autem facere aut cum. Dolorem, molestias animi nisi esse quam quo optio! Quidem nobis",
    'date' : 'March 17, 2025'
  },
 ];
 const speaking = [
  {
    'title': 'NY Economics Forum',
    'location': 'New York, NY',
    'date': 'August 25th 2025, 7:00pm'
  },
  {
    'title': 'Emerging Tech Meet-Up',
    'location': 'San Francisco, CA',
    'date': 'August 25th 2025, 7:00pm'
  },
  {
    'title': 'Creative Code Meetup',
    'location': 'Denver, CO',
    'date': 'August 25th 2025, 7:00pm'
  },
 ];
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
      <h1 class="tagline">I'm a <em>Scientist</em> and <em>Speaker</em> who is interested in the psychology of greed.</h1>
      <div class="two-column-section">
      <p>My Mission</p>
      <p>This is my mission. Maecenas a varius odio egestas auctor. Praesent facilisis, ex a gravida ultricies, quam sed megna placerat eros, et vehicula lectus ligula id dui. Aliquam uto cursus velit ut eros lorem ispum ullamcorper iaculis.</p>
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
  <section class="blog-section">
      <div class="blog-content">
          <div class="two-column-section">
              <p>Tech Blog</p>
              <div class="blog-posts">
                  <div v-for="value in blogs">
    <p class="blog-heading">{{value['heading']}}</p>
    <p class="blog-text">{{value['text']}}</p>
    <p class="blog-date">{{value['date']}}</p>
    </div>
              </div>
          </div>
      </div>
  </section>

  <section class="events-section">
      <div class="events-content">
          <div class="two-column-section">
              <p>Speaking Events</p>
              <div class="events-card">
                <div v-for="event in speaking">
                  <p class="event-title">{{event['title']}}</p>
                  <p class="event-location">{{event['location']}}</p>
                  <p class="event-date">{{event['date']}}</p>
                  </div>
              </div>
          </div>
      </div>
  </section>

  <footer>
      <div class="footer-content">
          <img src="./assets/instagram.png" alt="instagran">
          <img src="./assets/twitter.png" alt="twitter">
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
