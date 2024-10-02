<script setup>
import { defineProps } from 'vue';
const props = defineProps({
    speaking: {
        type: Array,
        required: true
    }
});
</script>
<template>
     <section class="events-section">
    <div class="events-content">
      <div class="two-column-section">
        <p>Speaking Events</p>
        <div class="events-card">
          <div v-for="event in speaking">
            <p class="event-title">{{ event.title }}</p>
            <p class="event-location">{{ event.location }}</p>
            <p class="event-date">{{ event.date }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>