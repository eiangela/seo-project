<template>
  <v-container class="pa-10">
    <v-row>
      <v-col cols="12" sm="6" md="4" lg="4">
        <h3 class="stick-footer-title font-weight-bold mb-5">Get in touch</h3>
        <h6 class="stick-footer-subtitle font-weight-black text-uppercase mb-5">
          We help you succeed online with proven SEO methods.
        </h6>
        <p class="stick-footer-text">
          Etiam sit amet convallis erat – class aptent taciti sociosqu ad litora
          torquent per conubia! Maecenas gravida lacus. Lorem etiam sit amet
          convallis erat.
        </p>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        md="4"
        lg="4"
        class="d-flex flex-column align-sm-center align-md-center"
      >
        <div>
          <h6
            class="stick-footer-contact-info text-uppercase font-weight-bold mb-5"
          >
            call us
          </h6>
          <p class="stick-footer-text">1 (234) 567-891</p>
          <p class="stick-footer-text">1 (234) 987-654</p>
        </div>
        <div>
          <h6
            class="stick-footer-contact-info text-uppercase font-weight-bold mt-5"
          >
            location
          </h6>
          <p class="stick-footer-text">
            121 Rock Sreet,<br />
            21 Avenue, <br />
            New York,<br />
            NY 92103-9000
          </p>
        </div>
        <div>
          <h6
            class="stick-footer-contact-info text-uppercase font-weight-bold mt-5"
          >
            top service
          </h6>
          <p class="stick-footer-text">SEO</p>
          <p class="stick-footer-text">Hosting</p>
        </div>
      </v-col>

      <v-col cols="12" sm="12" md="4" lg="4">
        <h3 class="stick-footer-title mb-5">Contact Us</h3>
        <v-form>
          <v-text-field
            variant="solo"
            density="compact"
            label="Enter your Name"
            single-line
          ></v-text-field>
          <v-text-field
            variant="solo"
            density="compact"
            label="Enter a valid email adress"
            single-line
          ></v-text-field>
          <v-textarea
            variant="solo"
            density="compact"
            label="Message"
            single-line
          ></v-textarea>
          <v-btn block class="stick-footer-btn font-weight-bold rounded-lg"
            >submit</v-btn
          >
        </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>
