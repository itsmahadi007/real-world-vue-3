<template>
  <div class="events">
    <img alt="Vue logo" src="../assets/logo.png" />
    <h4>This is home</h4>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
          id: 5928101,
          category: "animal welfare",
          title: "Cat Adoption Day",
          description: "Find your new feline friend at this event.",
          location: "Meow Town",
          date: "January 28, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Kat Laydee"
        },
        {
          id: 59281011,
          category: "animal welfare",
          title: "Cat Adoption Day",
          description: "Find your new feline friend at this event.",
          location: "Meow Town",
          date: "January 28, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Kat Laydee"
        },
        {
          id: 59281012,
          category: "animal welfare",
          title: "Cat Adoption Day",
          description: "Find your new feline friend at this event.",
          location: "Meow Town",
          date: "January 28, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "Kat Laydee"
        }
      ]
    };
  }
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
