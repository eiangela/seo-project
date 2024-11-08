<template>
  <div class="leadership-team pa-md-12">
    <div class="svg-background d-flex justify-center align-center">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 50 1440 200"
        class="background-svg"
      >
        <path
          fill="#f8dd28"
          fill-opacity="1"
          d="M0,224L0,0L1440,0L1440,320L0,320L0,320Z"
        ></path>
      </svg>

      <v-container>
        <v-row>
          <v-col
            cols="12"
            sm="4"
            md="4"
            v-for="(leaderInfo, index) in leadershipInfo"
            :key="index"
            :class="{ 'move-down': index === 1 }"
          >
            <v-card class="text-center rounded-xl">
              <v-avatar size="65" class="mt-5">
                <v-img :src="leaderInfo.leaderAvatar"> </v-img>
              </v-avatar>
              <v-card-text class="leadership-team-text font-weight-light">
                "{{ leaderInfo.text }}"
              </v-card-text>
              <v-card-title
                class="text-uppercase leadership-team-card-title mb-5"
              >
                {{ leaderInfo.name }} <br />
                <span class="font-weight-bold">{{ leaderInfo.jobTitle }}</span>
              </v-card-title>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script setup>
import imageNial from "@/assets/images/Untitled-1.jpg";
import imageMerry from "@/assets/images/ggg.jpg";
import imageFrank from "@/assets/images/sdasd.jpg";

const leadershipInfo = [
  {
    text: "Sample quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc",
    name: "Nill Smith",
    jobTitle: "Financial Director",
    leaderAvatar: imageNial,
  },
  {
    text: "Sample quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc",
    name: "Merry Kinnly ",
    jobTitle: "Chief Accountant",
    leaderAvatar: imageMerry,
  },
  {
    text: "Sample quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc",
    name: "Frank Kinney",
    jobTitle: "Sales Manager",
    leaderAvatar: imageFrank,
  },
];
</script>
