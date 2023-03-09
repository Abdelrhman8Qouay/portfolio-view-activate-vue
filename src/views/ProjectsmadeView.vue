<template>
  <!-- Start Projects  -->

  <div class="projectsCap mb-6">
    <!-- Title Row -->
    <div class="d-flex flex-md-row flex-sm-column justify-space-between">
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
        <div class="mainTit">{{ content.title }}</div>
        <div class="pros">
          <div
            class="proBox text-white"
            :key="k"
            v-for="(project, k) in content.content"
            data-aos="fade-down"
            data-aos-duration="2000"
          >
            <div class="mainCard">
              <div class="imgProB">
                <img :src="project.image" :alt="'project ' + k" />
              </div>
            </div>
            <div class="bodyCard">
              <div class="title">{{ project.name }}</div>
              <p>
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

const contentProjects = ref([
  { content: dataProjectsFront, title: "Front End" },
  { content: dataProjectsFull, title: "Full Stack" },
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

// Get Icons To Put It On { library } to get from it the icons
import { library } from "@fortawesome/fontawesome-svg-core";
import {
  faPaperPlane,
  faPanorama,
  faEye,
  faCode,
} from "@fortawesome/free-solid-svg-icons";
import { faFacebook } from "@fortawesome/free-brands-svg-icons";

library.add([faPaperPlane, faPanorama, faEye, faCode]);
library.add([faFacebook]);
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
      background: rgba(40, 40, 40, 0.437);
      padding: 5px;
      .mainTit {
        font-size: 1.9rem;
        color: #fff;
        font-weight: bold;
        text-align: center;
        position: relative;
        letter-spacing: 0.3rem;
        &::before {
          content: "";
          position: absolute;
          width: 100%;
          height: 2px;
          background: red;
          bottom: -3px;
          left: 0;
        }
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
            background-color: var(--body);
            z-index: 20;
            color: var(--for-word);
            .title {
              padding: 1rem;
              background-color: #222222;
              color: var(--for-addition);
              text-align: start;
            }

            p {
              padding: 1rem;
              color: var(--for-word);
              text-align: start;
            }

            .btnsCard {
              display: flex;
              padding: 1rem;
              justify-content: space-between;
              a {
                text-decoration: none;
                color: var(--for-word);
                background-color: var(--for-addition);
                padding: 7px 15px;
                display: flex;
                align-items: center;
                transition: 0.4s;

                &:hover {
                  color: var(--for-addition);
                  background-color: var(--for-word);
                }

                ion-icon {
                  margin-right: 10px;
                  font-size: inherit;
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