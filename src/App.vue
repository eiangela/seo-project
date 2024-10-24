<script setup>
import AppBar from "./components/AppBar.vue";
import HomeIndex from "./pages/HomeIndex.vue";
</script>

<template>
  <v-app>
    <header>
      <AppBar />
    </header>

    <v-main>
      <HomeIndex />
    </v-main>
  </v-app>
</template>
