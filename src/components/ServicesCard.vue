<template>
  <v-container>
    <h4 class="services-section-title font-weight-bold text-center">
      Development Services
    </h4>
    <p class="services-section-text text-center">
      Sample text. Click to select the text box. Click again or double click to
      start editing the text.
    </p>
    <v-row>
      <v-col
        v-for="service in seoServices"
        :key="service"
        cols="12"
        sm="6"
        md="6"
        lg="4"
        xl="4"
        xxl="4"
      >
        <v-card
          class="d-flex justify-center flex-column align-center pa-5 pa-md-10 rounded-xl"
        >
          <v-avatar class="services-card-avatar" size="80">
            <v-icon class="services-card-icon" size="50">
              {{ service.icon }}
            </v-icon>
          </v-avatar>
          <v-card-title
            class="services-card-title text-uppercase font-weight-bold text-center"
            >{{ service.title }}</v-card-title
          >
          <v-card-text class="services-card-text text-center">{{
            service.text
          }}</v-card-text>
          <v-card-actions>
            <v-btn
              class="services-card-btn rounded-pill font-weight-bold"
              width="80"
              height="40"
            >
              more</v-btn
            >
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const seoServices = [
  {
    title: "App Development",
    text: "Sample text. Click to select the text box. Click again or double click to start editing the text. Excepteur sint occaecat cupidatat non proident.",
    icon: "mdi-code-block-tags",
  },
  {
    title: "Mobility Services",
    text: "Sample text. Click to select the text box. Click again or double click to start editing the text. Excepteur sint occaecat cupidatat non proident.",
    icon: "mdi-cog-outline",
  },
  {
    title: "Consulting",
    text: "Sample text. Click to select the text box. Click again or double click to start editing the text. Excepteur sint occaecat cupidatat non proident.",
    icon: "mdi-nature-people-outline",
  },
  {
    title: "Team Extension",
    text: "Sample text. Click to select the text box. Click again or double click to start editing the text. Excepteur sint occaecat cupidatat non proident.",
    icon: "mdi-account-group",
  },
  {
    title: "Applications",
    text: "Sample text. Click to select the text box. Click again or double click to start editing the text. Excepteur sint occaecat cupidatat non proident.",
    icon: "mdi-cellphone-arrow-down",
  },
  {
    title: "24/7 Support",
    text: "Sample text. Click to select the text box. Click again or double click to start editing the text. Excepteur sint occaecat cupidatat non proident.",
    icon: " mdi-face-agent",
  },
];
</script>
