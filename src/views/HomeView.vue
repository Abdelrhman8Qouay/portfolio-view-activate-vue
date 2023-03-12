
<template>
  <div :class="themeColor.bg_main_darken" class="h-100">
    <!-- Landing Pro start -->
    <div class="landing">
      <v-container style="z-index: 10">
        <div class="rowLanding d-flex flex-md-row flex-sm-column">
          <v-col>
            <v-card
              class="mx-auto bg-transparent border-success"
              theme="dark"
              prepend-icon="fab fa-twitter"
              max-width="400"
              title="Hi all, I'am Abdelrhman"
            >
              <template v-slot:prepend>
                <v-icon size="x-large"></v-icon>
              </template>

              <v-card-text style="font-weight: 300" class="text-h6 py-2">
                Welcome Friends, this site same like a (pixel art) world, you
                can see my skills
              </v-card-text>

              <v-card-actions>
                <v-list-item class="w-100">
                  <template v-slot:prepend>
                    <v-btn
                      color="primary"
                      icon
                      @click="activeLocation = !activeLocation"
                      ><v-icon>fas fa-location-dot</v-icon></v-btn
                    >
                  </template>

                  <v-list-item-title>Open location</v-list-item-title>

                  <v-list-item-subtitle>activate</v-list-item-subtitle>

                  <template v-slot:append>
                    <v-btn
                      color="primary"
                      prepend-icon="fas fa-download"
                      @click="activeLocation = !activeLocation"
                      href="../../src/assets/cvOwner.pdf"
                      >Download CV</v-btn
                    >
                  </template>
                </v-list-item>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col class="d-flex justify-center">
            <div class="contentImg">
              <img
                src="../../src/assets/mePixelArt.jpg"
                alt="me"
                class="imgMain"
              />
            </div>
          </v-col>
        </div>
      </v-container>
    </div>
    <!-- Landing Pro end -->

    <!-- main start  -->
    <main>
      <!-- Location Box  -->
      <div class="contentLoc" :class="activeLocation ? 'active' : ''">
        <v-container>
          <div class="card-header d-flex justify-space-around my-5">
            <h2 :class="themeColor.spe_color_alot">
              <v-icon start>fas fa-map-location-dot</v-icon> Location
            </h2>
            <v-btn
              color="primary"
              append-icon="fas fa-xmark"
              @click="activeLocation = false"
              >Close</v-btn
            >
          </div>
          <div class="card-body">
            <div class="mapBox">
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d6901.504977575526!2d31.330718724027676!3d30.1298952274049!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x145815b411eed097%3A0x9f783c0b943765e6!2z2LnZitmGINi02YXYsyDYp9mE2LTYsdmC2YrYqdiMINmC2LPZhSDYudmK2YYg2LTZhdiz2Iwg2YXYrdin2YHYuNipINin2YTZgtin2YfYsdip4oCs!5e0!3m2!1sar!2seg!4v1663429237646!5m2!1sar!2seg"
                allowfullscreen=""
                loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"
              ></iframe>
            </div>
          </div>
        </v-container>
      </div>
      <!-- End Location Box -->

      <!-- Start About Us  -->
      <div class="containBoxUs">
        <v-container>
          <div
            class="aboutContent d-flex align-start justify-space-between flex-md-row flex-sm-column bg-transparent"
          >
            <div
              class="myInfo text-white rounded position-relative"
              :class="themeColor.bg_main"
              data-aos="fade-right"
              data-aos-duration="2000"
            >
              <div class="imgGl"></div>
              <h2 id="le" :class="themeColor.spe_color_alot">
                <v-icon start>fas fa-earth-africa</v-icon> About Us
              </h2>
              <p>
                <span :class="themeColor.spe_color_alot"
                  >Hi it's Me Abdelrhman Ashraf</span
                >, I am a Web developer based in Cairo, Egypt. I am very
                passionate about improving my coding skills & developing
                websites. Coming To Full Stack With PHP and Laravel. Working for
                myself to improve my skills. To be more precise most of my work
                is on the front end and I have completed most road map for it.
                The Next level of my ideas is Building a real projects with
                Python World.
              </p>
              <div class="inf d-flex w-100 flex-wrap">
                <p>
                  Age:
                  <span>{{ ownerAge }}</span>
                </p>
                <p>Email: <span>qouay555@gmail.com</span></p>
                <p>Phone: <span>0102 789 3028</span></p>
                <p>Place: <span> Cairo-Egypt Ain shams</span></p>
              </div>
            </div>
            <div class="imgInfo" data-aos="fade-left" data-aos-duration="2000">
              <img src="../../src/assets/robot.png" alt="robot" />
            </div>
          </div>
        </v-container>
      </div>
      <!-- End About Us  -->

      <!-- Start Education Box -->
      <div class="educationBox mb-3" :class="themeColor.bg_main">
        <v-container>
          <div class="my-5">
            <div class="pa-2">
              <h1
                class="border-double px-4 py-1 text-center"
                style="width: max-content"
                :class="themeColor.white_color"
              >
                <v-icon start>fas fa-graduation-cap</v-icon> My
                <span :class="themeColor.spe_color_alot">Education</span>
              </h1>
            </div>
            <p class="text-start px-4 py-1">
              Education Is Not The Learning Of Facts, But The Training Of The
              Mind To Think.
            </p>
          </div>
          <div class="restCollege">
            <v-card
              class="stCard"
              :class="themeColor.bg_main_darken"
              theme="dark"
            >
              <div class="d-flex flex-no-wrap justify-space-between">
                <div>
                  <v-avatar class="ma-3" size="125" rounded="0">
                    <v-img
                      src="https://www.elwekalanews.net/UploadCache/libfiles/13/5/600x338o/737.jpg"
                      alt="the institute"
                    ></v-img>
                  </v-avatar>

                  <div>
                    <v-card-title
                      class="text-h5"
                      :class="themeColor.spe_color_alot"
                      >Bachelor of Business Administration</v-card-title
                    >
                    <v-card-title class="text-h6 text-white"
                      >College of engineering, computer science and
                      management</v-card-title
                    >

                    <v-card-subtitle>2021-2025 | Pursuing</v-card-subtitle>
                  </div>
                </div>
              </div>
            </v-card>
            <div class="imgStudy">
              <img
                src="../../src/assets/imageKav/studying.gif"
                alt="girl studying pixel art"
              />
            </div>
          </div>
        </v-container>
      </div>
      <!-- End Education Box -->

      <!-- Start Skills  -->
      <div class="contentTeckSkills w-100">
        <v-container class="mb-4">
          <div class="pa-2">
            <h1
              class="border-double px-4 py-1 text-center"
              style="width: max-content"
              :class="themeColor.white_color"
            >
              <v-icon start>fas fa-toolbox</v-icon>Technologies
            </h1>
          </div>
          <div class="staticSkills">
            <div
              v-for="(skill, i) in dataSkills"
              :key="i"
              class="boxS"
              data-aos="fade-down"
              data-aos-duration="2000"
            >
              <div class="imgBox">
                <img :src="skill.image" :alt="skill.name" />
              </div>
              <p>{{ skill.name }}</p>
              <v-tooltip max-width="200" activator="parent" location="top">{{
                skill.describe
              }}</v-tooltip>
            </div>
          </div>
          <div class="movingSkills">
            <div class="teckSkill">
              <div class="pa-2">
                <h1
                  class="border-double px-4 py-1 text-center"
                  style="width: max-content"
                  :class="themeColor.white_color"
                >
                  <v-icon start>fas fa-anchor</v-icon> professional Skills
                </h1>
              </div>
              <p>Team Work</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="51%">0%</div>
              </div>

              <p>Performance Pages</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="43%">0%</div>
              </div>

              <p>Creativity</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="68%">0%</div>
              </div>

              <p>Communication</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="22%">0%</div>
              </div>

              <p>Project Management</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="25%">0%</div>
              </div>

              <p>Typing Speed</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="62%">0%</div>
              </div>

              <p>Problem Solving</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="46%">0%</div>
              </div>

              <p>Searching</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="76%">0%</div>
              </div>

              <p>Analysis</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="18%">0%</div>
              </div>

              <p>Debugging</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="41%">0%</div>
              </div>
            </div>
          </div>
          <div class="movingSkills">
            <div class="teckSkill">
              <div class="pa-2">
                <h1
                  class="border-double px-4 py-1 text-center"
                  style="width: max-content"
                  :class="themeColor.white_color"
                >
                  <v-icon start>fas fa-person-walking-luggage</v-icon>Working On
                </h1>
              </div>
              <p>Web Design</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="57%">0%</div>
              </div>

              <p>Web Front-end</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="74%">0%</div>
              </div>

              <p>Web Back-end</p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="34%">0%</div>
              </div>

              <p>
                Web API
                <span
                  data-bs-toggle="tooltip"
                  data-bs-placement="bottom"
                  title="working with falcon module"
                  ><ion-icon name="help-circle"></ion-icon
                ></span>
              </p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="66%">0%</div>
              </div>

              <p>
                Web Scraping
                <span
                  data-bs-toggle="tooltip"
                  data-bs-placement="bottom"
                  title="working with requests and beautifulSoup modules"
                  ><ion-icon name="help-circle"></ion-icon
                ></span>
              </p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="47%">0%</div>
              </div>

              <p>
                Automation
                <span
                  data-bs-toggle="tooltip"
                  data-bs-placement="bottom"
                  title="working with selenium module or others"
                  ><ion-icon name="help-circle"></ion-icon
                ></span>
              </p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="2%">0%</div>
              </div>

              <p>
                AI Work
                <span
                  data-bs-toggle="tooltip"
                  data-bs-placement="bottom"
                  title="working with tensorflow or opencv module or others"
                  ><ion-icon name="help-circle"></ion-icon
                ></span>
              </p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="1%">0%</div>
              </div>

              <p>
                Images Editor Programmer
                <span
                  data-bs-toggle="tooltip"
                  data-bs-placement="bottom"
                  title="working with pillow or mahotas module or others"
                  ><ion-icon name="help-circle"></ion-icon
                ></span>
              </p>
              <div class="containerTeckSkill">
                <div class="skills" style="width: 0" data-width="1%">0%</div>
              </div>
            </div>
          </div>
        </v-container>
      </div>
      <!-- End Skills  -->
    </main>

    <!-- main end  -->
  </div>
</template>

<script setup>
import dataSkills from "../data/dataSkills.json";
import { ref } from "vue";

const activeLocation = ref(false);
const ownerAge = ref(
  Math.floor(
    (new Date() - new Date("July 8, 2003 01:15:00")) / 1000 / 60 / 60 / 24 / 365
  )
);

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

// anonymous Function Onscroll For progress

window.onscroll = () => {
  const teckSkills = document.querySelectorAll(".containerTeckSkill .skills");
  // for move at down
  // moving each skill alone with scrolling
  teckSkills.forEach((skill) => {
    if (skill.getBoundingClientRect().top < 700) {
      skill.style.width = skill.dataset.width;
      skill.textContent = skill.dataset.width;
    } else if (skill.getBoundingClientRect().top > 700) {
      skill.style.width = "0";
      skill.textContent = "0%";
    }
  });
};
</script>


<style lang="scss" scoped>
/* Landing Start */
.landing {
  width: 100%;
  min-height: 80vh;
  background: url(../../src/assets/imageKav/backgroundLanding.webp);
  background-position: bottom;
  background-size: cover;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: row;
  position: relative;
  padding: 200px 0 100px 0;
  &::before {
    content: "";
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 70%;
    background: linear-gradient(0deg, #000 45%, transparent);
  }

  .rowLanding {
    min-height: 250px;

    .contentImg {
      max-width: 290px;
      height: 100%;
      clip-path: polygon(15% 1%, 100% 0, 100% 100%, 30% 100%, 0 48%);
      .imgMain {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
  }
}

/* Landing End  */

/* Start Location Box  */
.contentLoc {
  background-color: #41464b;
  transform-origin: top;
  transform: scaleY(0);
  position: absolute;
  opacity: 0;
  width: 100%;
  min-height: 350px;
  visibility: hidden;
  padding-top: 1rem;
  padding-bottom: 1rem;
  transition: 0.4s;
  box-shadow: inset 0 0 12px #000;

  &.active {
    transform: scaleY(1);
    visibility: visible;
    opacity: 1;
    position: static;
  }

  .card-body {
    height: 500px;
    .mapBox {
      padding: 1.3rem;
      box-shadow: 0 0 12px black, inset 0 0 12px black;
      border-radius: 5px;
      height: 100%;

      iframe {
        width: 100%;
        height: 100%;
        filter: invert(100%);
      }
    }
  }
}

/* End Location Box  */

/* Start About Us  */
.containBoxUs {
  background: url(../../src/assets/imageKav/rog-wallpaper-design-on-behance.gif);
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  background-position: bottom;
  padding: 5rem;

  .aboutContent {
    max-height: 400px;

    .imgInfo {
      height: 340px;
      img {
        width: 100%;
        height: 100%;
        object-fit: contain;
      }
    }

    .myInfo {
      max-width: 550px;
      box-shadow: 0 0 7px rgba(0, 0, 0, 0.4);
      padding: 1rem;
      h3 {
        font-weight: 600;
      }
      .imgGl {
        position: absolute;
        width: 80px;
        height: 80px;
        right: 5%;
        top: -15px;
        border-radius: 50%;
        background: url(https://i0.wp.com/www.lil-ye.com/wp-content/uploads/2020/10/Fantastic.gif?ssl=1&resize=1280%2C1280);
        background-size: 100%;
        border: 5px solid #011f74;
        &::before {
          content: "";
          position: absolute;
          top: 0;
          left: 0;
          width: 100%;
          height: 100%;
          border-radius: 50%;
          background: url(https://i0.wp.com/www.lil-ye.com/wp-content/uploads/2020/10/Fantastic.gif?ssl=1&resize=1280%2C1280);
          background-size: 100%;
          opacity: 0.5;
          mix-blend-mode: hard-light;
        }
        &:hover::before {
          animation: glitchAnim 0.2s linear infinite;
        }
      }

      p span {
        font-weight: 600;
        font-size: 1.3em;
        color: var(--for-spesh);
      }
      .inf {
        p {
          flex: 1 0 50%;
        }
        span {
          color: var(--spe-color);
          font-size: 13px;
        }
      }
    }
  }
}
@keyframes glitchAnim {
  0% {
    background-position: 0 0;
    filter: hue-rotate(0deg);
  }
  10% {
    background-position: 5px 0;
  }
  20% {
    background-position: -5px 0;
  }
  30% {
    background-position: 15px 0;
  }
  40% {
    background-position: 5px 0;
  }
  50% {
    background-position: -25px 0;
  }
  60% {
    background-position: -50px 0;
  }
  70% {
    background-position: 0 -20px;
  }
  80% {
    background-position: -60px -20px;
  }
  81% {
    background-position: 0 0;
  }
  100% {
    background-position: 0 0;
    filter: hue-rotate(360deg);
  }
}

/* End About Us  */

/* Start Moving Skills  */
.contentTeckSkills {
  .staticSkills {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-between;
    padding: 1rem;
    gap: 5rem;
    .boxS {
      background: url(https://studio.code.org/v3/assets/BPlVtb4JtsQ8ctmYwj7FNleFFG7JTeldTQmsHt7pz68/goldCoin.gif);
      background-position-x: 47%;
      background-position-y: 47%;
      width: 100px;
      height: 100px;
      border-radius: 50%;
      box-shadow: 0 0 12px rgba(0, 0, 0, 0.4);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 10px;
      transition: 0.4s;
      animation: FloatingBS 1s ease-in-out infinite alternate;
      position: relative;
      &:nth-child(even) {
        animation: FloatingRevBS 1s ease-in-out infinite alternate;
      }
      &:hover {
        animation-play-state: paused;
        box-shadow: 0 0 30px var(--for-addition);
      }

      .imgBox {
        display: block;
        width: 35px;
        height: 35px;
        img {
          object-fit: contain;
          width: 100%;
          height: 100%;
        }
      }

      p {
        color: #dc3535;
        font-weight: 600;
        font-size: 13px;
      }
    }
  }

  .movingSkills {
    position: relative;
    transition: 1s;
    .teckSkill {
      transform-style: preserve-3d;
      padding: 1.5rem;
      p {
        padding-left: 6rem;
        margin: 0;
        color: var(--for-word);
      }

      .containerTeckSkill {
        width: 100%;
        background-color: #e1e1e1;
        height: auto;
        padding: 10px;
        .skills {
          text-align: center;
          padding-bottom: 10px;
          color: var(--for-addition);
          font-size: 0.9em;
          background-image: linear-gradient(45deg, #6d6fd5, #0d6efd);
          height: 20px;
          transition: 1.2s;
          transition-timing-function: ease-in;
        }
      }
    }

    .proSkills {
      transform-style: preserve-3d;
      padding: 1.5rem;
      h3 {
        text-align: center;
        color: var(--for-spesh);
        font-weight: 600;
        font-family: var(--font-bold);
      }
    }
  }
}
@keyframes FloatingRevBS {
  100% {
    transform: translateY(-10px);
  }
}
@keyframes FloatingBS {
  100% {
    transform: translateY(10px);
  }
}

/* Start Education Box */
.educationBox {
  width: 100%;
  min-height: 300px;
  padding: 2rem;
  box-shadow: inset 0 0 8px #000;
  .restCollege {
    display: flex;
    flex-direction: row;
    justify-content: center;
    .stCard {
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
      margin: 1rem;
      transition: 0.4s;
      &:hover {
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.7);
      }
    }

    .imgStudy {
      flex: 1 1;
      border-radius: 7px;
      img {
        object-fit: contain;
        width: 100%;
        height: 100%;
        border-radius: 7px;
      }
    }
  }
}
/* End Education Box */
</style>