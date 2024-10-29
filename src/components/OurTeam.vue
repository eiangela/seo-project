<template>
  <v-container>
    <div class="d-flex justify-center align-center flex-column">
      <h4 class="text-center our-team-title mb-5">Our Team</h4>
      <p class="our-team-paragraph font-italic text-center mb-8">
        Glavrida for habitant morbi tristique senectus et netus et malesuada
        fames
      </p>
    </div>
    <v-row>
      <v-col cols="12" sm="6" md="6" lg="3" v-for="team in ourTeam" :key="team">
        <v-card class="pa-3 text-center">
          <v-img
            :src="team.image"
            aspect-ratio="1"
            class="rounded-circle mx-auto mb-5"
            max-width="250px"
            max-height="250px"
            cover
          ></v-img>
          <v-card-title class="our-team-card-title font-weight-bold">
            {{ team.title }}
          </v-card-title>
          <v-card-subtitle class="our-team-card-subtitle font-weight-black">{{
            team.subtitle
          }}</v-card-subtitle>
          <v-card-text class="our-team-card-text font-italic">{{
            team.text
          }}</v-card-text>
          <v-card-actions class="d-flex justify-center">
            <v-btn
              v-for="icon in team.icons"
              :key="icon.name"
              :href="icon.link"
              elevation="0"
              target="_blank"
              icon
              text
            >
              <v-icon class="our-team-icon">{{ icon.name }}</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import teamImage1 from "@/assets/images/dg.jpg";
import teamImage2 from "@/assets/images/gf1.jpg";
import teamImage3 from "@/assets/images/gggg.jpg";
import teamImage4 from "@/assets/images/fsr.jpg";

const socialIcons = [
  { name: "mdi-instagram", link: "https://instagram.com/example" },
  { name: "mdi-twitter", link: "https://twitter.com/example" },
  { name: "mdi-facebook", link: "https://facebook.com/example" },
];

const ourTeam = [
  {
    image: teamImage1,
    title: "Jeffrey Brown",
    subtitle: "creative leader",
    text: "Glavi amet ritnisl libero molestie ante ut fringilla purus eros quis glavrid from dolor amet iquam lorem bibendum",
    icons: socialIcons,
  },
  {
    image: teamImage2,
    title: "Ann Richmond",
    subtitle: "sales manager",
    text: "Glavi amet ritnisl libero molestie ante ut fringilla purus eros quis glavrid from dolor amet iquam lorem bibendum",
    icons: socialIcons,
  },
  {
    image: teamImage3,
    title: "Alex Greenfield",
    subtitle: "developer",
    text: "Glavi amet ritnisl libero molestie ante ut fringilla purus eros quis glavrid from dolor amet iquam lorem bibendum",
    icons: socialIcons,
  },
  {
    image: teamImage4,
    title: "May Smith",
    subtitle: "web designer",
    text: "Glavi amet ritnisl libero molestie ante ut fringilla purus eros quis glavrid from dolor amet iquam lorem bibendum",
    icons: socialIcons,
  },
];
</script>
