<script setup>
import VHeader from "./components/VHeader.vue";
import VPromo from "./components/VPromo.vue";
import VClassroom from "./components/VClassroom.vue";
import VHistory from "./components/VHistory.vue";
import VPossibilties from "./components/VPossibilities.vue";
import VIdea from "./components/VIdea.vue";
import VReviews from "./components/VReviews.vue";
import VFooter from "./components/VFooter.vue";
</script>

<template>
  <v-Header />
  <main>
    <v-Promo />
    <v-Classroom />
    <v-History />
    <v-Possibilties />
    <v-Idea />
    <v-Reviews />
  </main>
  <v-Footer />
</template>

<style scoped>
</style>
