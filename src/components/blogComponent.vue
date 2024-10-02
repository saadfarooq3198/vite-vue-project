<script setup>
import  { defineProps } from 'vue';
const props = defineProps({
   blogs: {
      type: Array,
      Required: true
   },
});
</script>
<template>
   <section class="blog-section">
    <div class="blog-content">
      <div class="two-column-section">
        <p>Tech Blog</p>
        <div class="blog-posts">
          <div v-for="blog in blogs">
            <p class="blog-heading">{{ blog.heading }}</p>
            <p class="blog-text">{{ blog.text }}</p>
            <p class="blog-date">{{ blog.date }}</p>
          </div>
        </div>
      </div>
    </div>
  </section> 
</template>