<script setup>
import SeoIntro from "../components/SeoIntro.vue";
import OurConsulting from "../components/OurConsulting.vue";
import ServicesCard from "../components/ServicesCard.vue";
</script>

<template>
  <section class="seo-intro">
    <div class="background-image"></div>

    <div class="content-wrapper">
      <SeoIntro />
    </div>
  </section>

  <section class="our-consulting">
    <OurConsulting />
  </section>

  <section class="services-card">
    <ServicesCard />
  </section>
</template>
