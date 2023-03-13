<template>
  <!-- Start Projects  -->

  <div class="projectsCap mb-6">
    <!-- Title Row -->
    <div
      class="d-flex flex-md-row flex-sm-column justify-space-between pa-2"
      :class="themeColor.bg_main_darken"
    >
      <a
        class="btnRepo px-4 py-1 border-double"
        href="https://github.com/Abdelrhman8Qouay?tab=repositories"
        ><img
          src="../../src/assets/Icons/githupPixelArtPng.png"
          class="imgBtnRepo"
        />
        Show All Repos</a
      >
      <h1 class="border-double px-4 py-1" :class="themeColor.white_color">
        Projects Made
      </h1>
    </div>
    <!-- Title Row -->

    <!-- Main Content -->
    <div class="testGrill">
      <!-- Content All Types Of Projects -->
      <div
        :key="i"
        v-for="(content, i) in contentProjects"
        class="contentTable my-4"
      >
        <div class="mainTit" :class="themeColor.white_color">
          {{ content.title }}
        </div>
        <div class="pros">
          <div
            class="proBox text-white"
            :key="k"
            v-for="(project, k) in content.content"
            data-aos="fade-down"
            data-aos-duration="2000"
          >
            <div
              v-if="project.info != ''"
              :class="badgeBackgroundColors[project.info]"
              class="badge_card text-red pa-2 position-absolute rounded"
              style="z-index: 18; position: relative; top: 5%; left: 5%"
            >
              {{ project.info }}
            </div>
            <div class="mainCard">
              <div class="imgProB">
                <img
                  :src="
                    project.image == ''
                      ? getImageUrl('assets/projects/undifBack.png')
                      : getImageUrl(project.image)
                  "
                  :alt="'project ' + k"
                />
              </div>
            </div>
            <div class="bodyCard" :class="themeColor.bg_main_light">
              <div class="title text-white" :class="themeColor.bg_main_darken">
                {{ project.name }}
              </div>
              <div
                class="action_carding d-flex flex-column h-75 justify-space-between"
              >
                <p class="overflow-auto h-100" :class="themeColor.spe_color">
                  {{ project.describe }}
                </p>
                <div class="btnsCard">
                  <a :href="project.viewPage"
                    ><v-icon class="me-2" size="20">fas fa-eye</v-icon> View</a
                  >
                  <a :href="project.codePage"
                    ><v-icon class="me-2" size="20">fas fa-code</v-icon> Code</a
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- FrontEnd Projects -->
    </div>
    <!-- Main Content -->
  </div>
  <!-- End Projects  -->
</template>

<script setup>
import dataProjectsFront from "../data/dataProjectsFront.json";
import dataProjectsFull from "../data/dataProjectsFull.json";
import { ref } from "vue";

// Variables Option
const onboarding = ref(false);
const badgeBackgroundColors = ref({
  pending: "bg-warning",
  completed: "bg-success",
  updated: "bg-primary",
});

const contentProjects = ref([
  { content: dataProjectsFront, title: "Front End" },
  { content: dataProjectsFull, title: "Full Stack" },
]);

const contentRecommended = ref([
  dataProjectsFront[2],
  dataProjectsFront[3],
  dataProjectsFront[4],
]);

const themeColor = ref({
  bg_main_light: "bg-blue-grey-darken-1",
  bg_main: "bg-blue-grey-darken-3",
  bg_main_darken: "bg-blue-grey-darken-4",

  bg_spe_color: "bg-cyan-lighten-1",

  bg_black_color: "bg-black",
  black_color: "text-black",

  spe_color: "text-cyan-lighten-1",
  spe_color_alot: "text-indigo",
  white_color: "text-white",
});

function getImageUrl(urlName) {
  return new URL(`../${urlName}`, import.meta.url).href;
}
</script>

<style lang="scss" scoped>
/* Start Projects  */
.projectsCap {
  width: 100%;
  height: 100%;
  padding: 20px;
  background: url(https://i.pinimg.com/originals/b8/2f/28/b82f28a7e9c8fcb3868d3d94652c107c.gif);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;

  .btnRepo {
    text-decoration: none;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 7px;
    font-size: 1.4rem;
    font-weight: bold;
    color: #fff;
    &:hover {
      color: var(--active-color);
    }
    .imgBtnRepo {
      width: 45px;
      height: 45px;
      object-fit: cover;
    }
  }

  // Main Content
  .testGrill {
    display: flex;
    flex-direction: column;
    gap: 10px;

    .contentTable {
      background: var(--smooth-bg);
      padding: 5px;
      .mainTit {
        font-size: 1.9rem;
        font-weight: bold;
        text-align: center;
        position: relative;
        letter-spacing: 0.3rem;
        text-decoration: underline;
      }
      .pros {
        display: flex;
        flex-wrap: wrap;
        text-align: center;
        justify-content: space-between;
        gap: 10px;
        .proBox {
          position: relative;
          flex: 1 0 400px;
          max-width: 400px;
          max-height: 200px;
          overflow: hidden;
          border-radius: 5px;

          &:hover .bodyCard {
            top: 0%;
          }

          .mainCard {
            .imgProB {
              width: 100%;
              height: 100%;
              position: absolute;
              left: 0;
              top: 0;

              img {
                width: 100%;
                height: 100%;
                object-fit: cover;
              }
            }
          }
          .bodyCard {
            position: relative;
            transition: 0.4s;
            top: 75%;
            width: 100%;
            height: 100%;
            z-index: 20;
            .title {
              padding: 1rem;
              background-color: #222222;
              text-align: start;
            }

            p {
              padding: 1rem;
              text-align: start;
            }

            .btnsCard {
              display: flex;
              padding: 1rem;
              justify-content: space-between;
              a {
                text-decoration: none;
                color: #fff;
                padding: 7px 15px;
                display: flex;
                align-items: center;
                transition: 0.4s;
                &:hover {
                  color: var(--active-color);
                }
              }
            }
          }
        }
      }
    }
  }
  // Main Content
}

/* End Projects  */
</style>