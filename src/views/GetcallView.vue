<template>
  <!-- Start Contact Touch -->
  <div class="contactTouch">
    <v-container>
      <div class="pa-2" :class="themeColor.bg_main_darken">
        <h1
          class="border-double px-4 py-1 text-center w-25"
          :class="themeColor.white_color"
        >
          Get In <span :class="themeColor.spe_color_alot">Touch</span>
        </h1>
      </div>
      <div class="contentTouch">
        <form
          class="contactBox d-flex align-start flex-column rounded pa-10"
          :class="themeColor.bg_main_darken"
          style="gap: 1rem; max-width: 450px"
          action="https://formspree.io/f/xwkjpygk"
          method="POST"
          data-aos="fade-down"
          data-aos-duration="2000"
        >
          <v-text-field
            color="cyan-lighten-1"
            type="text"
            clearable
            label="Name"
            name="name"
            prepend-inner-icon="fas fa-user"
            required
          ></v-text-field>
          <v-text-field
            color="cyan-lighten-1"
            prepend-inner-icon="fas fa-envelope"
            type="email"
            clearable
            label="Email"
            name="email"
            required
          ></v-text-field>
          <v-text-field
            color="cyan-lighten-1"
            prepend-inner-icon="fas fa-phone"
            type="text"
            clearable
            label="Phone"
            name="phone"
          ></v-text-field>
          <v-textarea
            color="cyan-lighten-1"
            name="message"
            rows="6"
            clearable
            label="Message"
            prepend-inner-icon="fas fa-message"
          ></v-textarea>
          <v-card-action>
            <v-btn
              color="primary"
              class="me-4"
              type="submit"
              name="send"
              @click="sendingSound.play()"
            >
              send now
            </v-btn>
          </v-card-action>
        </form>
      </div>
    </v-container>
  </div>
  <!-- End Contact Touch  -->
</template>

<script setup>
import { ref } from "vue";

const themeColor = ref({
  bg_main_light: "bg-blue-grey-darken-1",
  bg_main: "bg-blue-grey-darken-3",
  bg_main_darken: "bg-blue-grey-darken-4",

  bg_spe_color: "bg-cyan-lighten-1",

  bg_black_color: "bg-black",
  black_color: "text-black",

  spe_color: "text-cyan-lighten-1",
  spe_color_alot: "text-success",
  white_color: "text-white",
});

// add the audio for any where in the page'
var sendingSound = new Audio("../../src/assets/audios/notificationSending.mp3");
</script>

<style lang="scss" scoped>
/* Start Contact Touch */
.contactTouch {
  background: url(https://64.media.tumblr.com/75ee871c3c70501014511f527b342213/74bb6bc1ad2987d5-a1/s1280x1920/ae89e529ec10b97daff14c6aa3db56e663fbe416.gifv);
  background-size: cover;
  background-attachment: fixed;
  background-repeat: no-repeat;
  width: 100%;
  min-height: 400px;
  padding: 1rem;

  .contentTouch {
    padding: 3rem;
    padding-left: 0;
  }
}
.contactTouch h2 {
  background: var(--body);
  border-radius: 5px;
  padding: 10px;
}

.contactTouch .contentTouch {
  form {
    .v-text-field {
      width: 100%;
    }
    .v-textarea-field {
      width: 100%;
    }
  }
}
/* End Contact Touch */
</style>
