<script setup>
import SeoIntro from "../components/SeoIntro.vue";
import OurConsulting from "../components/OurConsulting.vue";
import ServicesCard from "../components/ServicesCard.vue";
import BrandPower from "../components/BrandPower.vue";
import OurTeam from "../components/OurTeam.vue";
import FrequentlyAskedQuestions from "../components/FrequentlyAskedQuestions.vue";
import LeadershipTeam from "../components/LeadershipTeam.vue";
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

  <section class="brand-power">
    <BrandPower />
  </section>

  <section class="our-team">
    <OurTeam />
  </section>

  <section class="frequently-asked-questions">
    <FrequentlyAskedQuestions />
  </section>

  <section class="leadership-team">
    <LeadershipTeam />
  </section>
</template>
