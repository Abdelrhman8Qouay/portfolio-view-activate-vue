
<template>
  <v-app id="inspire">
    <v-navigation-drawer
      style="background: linear-gradient(45deg, #41464b, #b41699, #ffdf4a)"
      expand-on-hover
      rail
      v-model="drawer"
    >
      <v-list>
        <v-list-item
          prepend-avatar="../src/assets/bussinLogo.png"
          title="Abdelrhman Ashraf"
          subtitle="qouay555@gmail.com"
          href="https://www.facebook.com/profile.php?id=100090009622327"
        ></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item
          prepend-icon="fas fa-user-secret"
          color="primary"
          title="Landing Pro"
          value="landing"
          to="/"
        ></v-list-item>
        <v-list-item
          prepend-icon="fas fa-project-diagram"
          title="Projects Made"
          value="projects"
          color="primary"
          to="projects"
        ></v-list-item>
        <v-list-item
          prepend-icon="fas fa-paper-plane"
          title="Get In Touch"
          color="primary"
          value="callme"
          to="getintouch"
        ></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar :class="themeColor.bg_main_light">
      <v-app-bar-nav-icon
        color="success"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>

      <v-toolbar-title :class="themeColor.spe_color"
        >AbdelrhmanQouay's
        <span :class="themeColor.spe_color_alot"
          >Portfolio</span
        ></v-toolbar-title
      >
    </v-app-bar>

    <v-main>
      <RouterView />
    </v-main>

    <div class="windowContent">
      <div class="upCon"></div>
      <div class="imging"></div>
      <div class="downCon"></div>
    </div>
    <v-footer
      class="flex-column"
      :class="themeColor.bg_main_light + ' ' + themeColor.white_color"
    >
      <!-- Grid container -->
      <v-container class="px-5 py-5 main">
        <!--Grid row-->
        <v-row>
          <!--Grid column-->
          <v-col cols="6" md="6" xs="12" class="mb-4 mb-md-0 contentMain">
            <h4
              class="text-uppercase text-xs-h4 text-md-h3"
              :class="themeColor.spe_color_alot"
              data-aos="fade-down"
              data-aos-duration="2000"
              style="font-weight: bold"
            >
              <span :class="themeColor.spe_color">Abdelrhman's</span>
              Portfolio
            </h4>

            <p>
              Thank you for visiting my personal portfolio website. Connect with
              me over socials.
              <br />
              <br />
              Keep Rising 🚀.
            </p>
          </v-col>
          <!--Grid column-->

          <!--Grid column-->
          <v-col cols="6" md="6" xs="12" class="mb-4 mb-md-0">
            <v-list class="bg-transparent" :lines="false" density="compact" nav>
              <v-list-subheader :class="themeColor.white_color"
                >CONTACT ME</v-list-subheader
              >

              <v-list-item
                v-for="(item, i) in itemsContact"
                :key="i"
                item-props
                lines="one"
              >
                <template v-slot:prepend>
                  <v-icon :icon="item.icon"></v-icon>
                </template>

                <v-list-item-title v-text="item.text"></v-list-item-title>
              </v-list-item>
            </v-list>
          </v-col>
          <!--Grid column-->
        </v-row>
        <!--Grid row-->
      </v-container>
      <!-- Grid container -->

      <!-- Copyright -->
      <div class="text-center w-100 px-5 py-5" :class="themeColor.bg_main">
        Designed With 💖 By
        <a
          href="https://www.facebook.com/profile.php?id=100090009622327"
          class="text-decoration-none"
          :class="themeColor.spe_color_alot"
          >Abdelrhman Ashraf</a
        >
        | all rights reserved © {{ new Date().getFullYear() }}
      </div>
      <!-- Copyright -->
    </v-footer>
  </v-app>
</template>

<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import { ref } from "vue";

const drawer = ref(false);

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

const itemsContact = ref([
  { icon: "fas fa-phone", text: "0102 789 3028" },
  { icon: "fas fa-envelope", text: "qouay555@gmail.com" },
  { icon: "fas fa-map-location-dot", text: "Egypt, cairo - ain_shams" },
]);
const itemsQuick = ref([
  { hre: "#", icon: "fas fa-arrow-right-to-bracket", text: "Landing" },
  { hre: "#le", icon: "fas fa-arrow-right-to-bracket", text: "About Us" },
  {
    hre: "#education",
    icon: "fas fa-arrow-right-to-bracket",
    text: "My Education",
  },
]);

// add the audio for any where in the page'
const onlineSound = new Audio("../../src/assets/audios/notification1.mp3");
window.ononline = () => {
  onlineSound.play();
};

// To Add Icons On This Page >>>>>
// this is must have
// Get Icons To Put It On { library } to get from it the icons
import { library } from "@fortawesome/fontawesome-svg-core";
import {
  faPaperPlane,
  faProjectDiagram,
  faUserSecret,
  faPhone,
  faEnvelope,
  faMapLocationDot,
  faArrowRightToBracket,
  faPanorama,
  faEye,
  faCode,
  faUser,
  faMessage,
  faDownload,
  faXmark,
  faEarthAfrica,
  faGraduationCap,
  faToolbox,
  faAnchor,
  faPersonWalkingLuggage,
} from "@fortawesome/free-solid-svg-icons";
import {
  faFacebook,
  faGithub,
  faTwitter,
  faLinkedin,
} from "@fortawesome/free-brands-svg-icons";

library.add([
  faPaperPlane,
  faProjectDiagram,
  faUserSecret,
  faPhone,
  faEnvelope,
  faMapLocationDot,
  faArrowRightToBracket,
  faPanorama,
  faEye,
  faCode,
  faUser,
  faMessage,
  faDownload,
  faXmark,
  faEarthAfrica,
  faGraduationCap,
  faToolbox,
  faAnchor,
  faPersonWalkingLuggage,
]);
library.add([faFacebook, faGithub, faTwitter, faLinkedin]);
</script>


<style lang="scss" scoped>
// Start Window
.windowContent .upCon {
  width: 100%;
  min-height: 150px;
  background-color: #41464b;
  box-shadow: inset 0 0 12px;
}
.windowContent .downCon {
  width: 100%;
  min-height: 150px;
  background-color: #41464b;
  box-shadow: inset 0 0 12px;
}
.windowContent .imging {
  width: 100%;
  background: url(https://i.pinimg.com/originals/a3/c3/77/a3c3776b73f2ac4aa70ba7db2a5f66f6.gif);
  min-height: 100px;
  background-size: initial;
  background-position: right;
}
// End Window
</style>
