<template>
  <div class="container mx-auto">
    <Header />
    <main class="">
      <TheHero />
      <TheCta id="program" />
      <TheBrends id="partners" />
      <TheSummit id="incentives" />
      <TheStatistic />
      <Register id="register" />
    </main>
  </div>
</template>

<script setup>
import TheStatistic from "./components/TheStatistic.vue";
import Header from "./components/Header.vue";
import TheHero from "./components/TheHero.vue";
import TheCta from "./components/TheCta.vue";
import TheBrends from "./components/TheBrends.vue";
import TheSummit from "./components/TheSummit.vue";
import Register from "./components/Register.vue";
</script>

<style lang="scss" scoped></style>
