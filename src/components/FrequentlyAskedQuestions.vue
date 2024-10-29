<template>
  <v-container>
    <v-row>
      <v-col>
        <div class="faq-asked-title text-center font-weight-bold mb-10">
          Frequently Asked Questions
          <div class="mx-auto my-2" style="max-width: 100px">
            <v-divider
              :thickness="6"
              class="border-opacity-100 mt-5"
              width="100"
            ></v-divider>
          </div>
        </div>

        <v-expansion-panels class="my-4 faq-asked-expan" variant="popout">
          <v-expansion-panel
            v-for="(faq, index) in faqInfo"
            :key="index"
            class="faq-asked-expan__wrapper rounded-xl"
          >
            <v-expansion-panel-title
              class="faq-asked-panel-title font-weight-black"
            >
              {{ faq.question }}
            </v-expansion-panel-title>

            <v-expansion-panel-text class="faq-asked-panel-text">
              {{ faq.answer }}
            </v-expansion-panel-text>
          </v-expansion-panel>
        </v-expansion-panels>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const faqInfo = [
  {
    question: "What if I need more time after the free trial?",
    answer:
      "Answer. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.",
  },
  {
    question: "Can I connect my domain name?",
    answer:
      "Answer. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.",
  },
  {
    question: "Do I need any design or coding skills?",
    answer:
      "Answer. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.",
  },
  {
    question: "Isn’t this similar to a reminders app?",
    answer:
      "Answer. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.",
  },
  {
    question: "Isn’t this similar to a reminders app?",
    answer:
      "Answer. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.",
  },
  {
    question: "Isn’t this similar to a reminders app?",
    answer:
      "Answer. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id suscipit ex. Suspendisse rhoncus laoreet purus quis elementum. Phasellus sed efficitur dolor, et ultricies sapien. Quisque fringilla sit amet dolor commodo efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.",
  },
];
</script>
