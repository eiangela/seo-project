<script setup>
import AppBar from "./components/AppBar.vue";
import HomeIndex from "./pages/HomeIndex.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <v-app>
    <header>
      <AppBar />
    </header>

    <v-main>
      <HomeIndex />
    </v-main>

    <footer class="sticky-footer">
      <Footer />
    </footer>
  </v-app>
</template>
