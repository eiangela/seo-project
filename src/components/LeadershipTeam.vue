<template>
  <v-container>
    <v-row>
      <v-col v-for="(leaderInfo, index) in leadershipInfo" :key="index">
        <v-card>
          <v-avatar>Avatar aqui</v-avatar>
          <v-card-text>{{ leaderInfo.text }}</v-card-text>
          <v-card-title>{{ leaderInfo.name }}</v-card-title>
          <span> {{ leaderInfo.jobTitle }}</span>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const leadershipInfo = [
  {
    text: "Sample quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc",
    name: "Nill Smith",
    jobTitle: "Financial Director",
  },
  {
    text: "Sample quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc",
    name: "Merry Kinnly ",
    jobTitle: "Chief Accountant",
  },
  {
    text: "Sample quote. Lorem ipsum dolor sit amet, consectetur adipiscing elit nullam nunc",
    name: "Frank Kinney",
    jobTitle: "Sales Manager",
  },
];
</script>
