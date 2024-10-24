<template>
  <v-app-bar :elevation="0">
    <v-row>
      <v-col class="d-flex align-center justify-center">
        <img
          src="../assets/images/ttt.png"
          class="logo-bar"
          alt="Logo"
          width="60"
        />
      </v-col>

      <v-col class="d-flex justify-center">
        <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      </v-col>
    </v-row>
  </v-app-bar>

  <v-navigation-drawer
    class="app-drawer"
    v-model="drawer"
    :location="$vuetify.display.mobile ? 'bottom' : undefined"
    temporary
  >
    <v-list :items="items"></v-list>
  </v-navigation-drawer>
</template>

<script setup>
import { ref, watch } from "vue";

const drawer = ref(false);
const group = ref(null);

const items = ref([
  {
    title: "Foo",
    value: "foo",
  },
  {
    title: "Bar",
    value: "bar",
  },
  {
    title: "Fizz",
    value: "fizz",
  },
]);

watch(group, () => {
  drawer.value = false;
});
</script>
