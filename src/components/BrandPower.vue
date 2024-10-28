<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="12" md="12" lg="6">
        <h4 class="brand-power-title mb-8">How we create brand power</h4>
        <ul
          v-for="info in informationBrand"
          :key="info"
          class="brand-power-list"
        >
          <li class="brand-power-list__item mt-3">{{ info.textBrand }}</li>
        </ul>
        <div class="brand-power-circle rounded-circle"></div>
      </v-col>

      <v-col
        cols="12"
        sm="12"
        md="12"
        lg="6"
        class="d-flex justify-md-center align-center mt-8"
      >
        <img class="brand-power-image" src="../assets/images/-min.jpg" alt="" />
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const informationBrand = [
  {
    textBrand: "We illuminate and cultivate the tensions that matter.",
  },
  {
    textBrand:
      "We copy, collect, and recut the best across culture and category.",
  },
  {
    textBrand:
      "We fine-tune the most compelling tensions, teasing out the right questions to ask.",
  },
  {
    textBrand:
      "We design potent and powerful solutions that drive meaning and memory.",
  },
];
</script>
