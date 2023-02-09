<script setup>
import Home_banner from "../components/Home_banner.vue";
import Home_newsSection from "../components/Home_newsSection.vue";
import Home_concept from "../components/Home_concept.vue";
import Home_menu from "../components/Home_menu.vue";
import Home_fqa from "../components/Home_fqa.vue";
import Home_information from "../components/Home_information.vue";
</script>

<template>
  <Home_banner></Home_banner>
  <main>
    <Home_newsSection></Home_newsSection>
    <Home_concept></Home_concept>
    <Home_menu></Home_menu>
    <Home_fqa></Home_fqa>
    <Home_information></Home_information>
  </main>
</template>
