<script setup>
import EventCard from "../components/EventCard.vue";
import { ref } from "vue";

const events = ref([{
  id: 1,
  category: 'animal welfare',
  title: 'cat adoption day',
  dedscription: 'find your feline friend at this event',
  location: 'meow town',
  date: 'january 28, 2022',
  time: '12:00',
  petsAllowed: true,
  organizer: 'kat laydee'
},
{
  id: 2,
  category: 'animal welfare',
  title: 'community gardening',
  dedscription: 'find your feline friend at this event',
  location: 'meow town',
  date: 'january 28, 2022',
  time: '12:00',
  petsAllowed: true,
  organizer: 'kat laydee'
},
{
  id: 3,
  category: 'animal welfare',
  title: 'beach cleanup',
  dedscription: 'find your feline friend at this event',
  location: 'meow town',
  date: 'january 28, 2022',
  time: '12:00',
  petsAllowed: true,
  organizer: 'kat laydee'
}],
)
</script>

<template>
  <h1>Events for good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event"></EventCard>
  </div>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>