
<template>
  <div class="containAllAbove">
    <!-- for Color -->
    <div class="colorMode">
      <ion-icon name="power"></ion-icon>
    </div>

    <!-- for Location  -->
    <div class="LocationBtn">
      <ion-icon name="location"></ion-icon>
    </div>

    <!-- <div class="headCont left_head">
                <div class="contentHeader">
                    <ul class="ulHeader">
                        <li><a class="link" href="#le">About Us</a></li>
                        <li><a class="link" href="#ld">Skills</a></li>
                        <li><a class="link" href="#foot">Projects</a></li>
                        <li><a class="link" href="#foot">Contact</a></li>
                    </ul>
                    <button class="up-to"><ion-icon name="caret-up"></ion-icon></button>
                    <button class="down-to"><ion-icon name="caret-down"></ion-icon></button>
                </div>
            </div> -->
    <!-- header end -->

    <!-- Start Titling  -->
    <div class="containTit flex-fill">
      <div class="titling">
        <div class="imgTit">
          <img src="../assets/mePixelArt.jpg" alt="me : owner" />
        </div>
        <div class="infTit">
          <h3>Hello there, I'am Abdelrhman Ashraf</h3>
          <p>
            i'am Web Developer more accurate Front End dev & MEVN Stack & Web
            Designing, you can hire me and also can download CV
          </p>
          <div class="btns d-flex">
            <button class="cvBtn px-4 py-1" style="margin-left: 20px">
              <a href="./assets/cvOwner.pdf">Download CV</a>
              <ion-icon name="disc"></ion-icon>
              <div class="toolMsg">Download CV</div>
            </button>
          </div>
        </div>
        <div class="star star1"></div>
        <div class="star star2"></div>
        <div class="star star3"></div>
        <div class="star star4"></div>
        <div class="star star5"></div>
        <div class="star star6"></div>
        <div class="star star7"></div>
        <div class="star star8"></div>
      </div>
    </div>
    <!-- End Titling  -->

    <div class="headCont right_head">
      <div class="contentHeader">
        <ul>
          <li>
            <a href="https://github.com/qouaynt"
              ><ion-icon name="logo-github"></ion-icon
            ></a>
          </li>
          <li>
            <a href="https://www.linkedin.com/in/abdelrhman-ashraf-222957220/"
              ><ion-icon name="logo-linkedin"></ion-icon
            ></a>
          </li>
        </ul>
        <!-- <button class="up-to"><ion-icon name="caret-up"></ion-icon></button>
                    <button class="down-to"><ion-icon name="caret-down"></ion-icon></button> -->
      </div>
    </div>
  </div>
  <!-- containAllAbove end  -->

  <div class="partUp"></div>

  <!-- main start  -->
  <main>
    <!-- Location Box  -->
    <div class="contentLoc">
      <div class="container">
        <div class="card-header">
          <h2><ion-icon name="location"></ion-icon> Location</h2>
          <ion-icon class="closeLocation" name="close"></ion-icon>
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
      </div>
    </div>
    <!-- End Location Box -->

    <!-- Start About Us  -->
    <div class="containBoxUs">
      <div class="container">
        <div class="aboutContent">
          <div class="myInfo" data-aos="fade-right" data-aos-duration="2000">
            <div class="imgGl"></div>
            <h2 id="le"><ion-icon name="planet"></ion-icon> About Us</h2>
            <p>
              <span>i'am living in Egypt, My city is Cairo</span>, I am a
              Front-End developer based in Cairo, Egypt. I am very passionate
              about improving my coding skills & developing websites. I build
              WebApps and Websites using MEVN Stack. Working for myself to
              improve my skills. Love to build Design of Page as UI and a little
              UX.
            </p>
            <div class="inf">
              <p>Age: <span>20</span></p>
              <p>Email: <span>mido59478@gmail.com</span></p>
              <p>Phone: <span>0102 789 3028</span></p>
              <p>Place: <span> Cairo-Egypt Ain shams</span></p>
            </div>
          </div>
          <div class="imgInfo" data-aos="fade-left" data-aos-duration="2000">
            <img src="./assets/robot.png" alt="robot" />
          </div>
        </div>
      </div>
    </div>
    <!-- End About Us  -->

    <div class="bordCl"></div>

    <!-- Start Skills  -->
    <div class="contentTeckSkills">
      <div class="container mb-4">
        <h2 id="skill">
          <ion-icon name="code-working"></ion-icon> Skills & Abilities
        </h2>
        <div class="staticSkills">
          <!-- <div class="boxS" data-aos="fade-down" data-aos-duration="2000" data-bs-toggle="tooltip" data-bs-placement="bottom" title="Tooltip on top">
                            <div class="imgBox">
                                <img src="./assets/Icons/bootstrap-5-logo-icon.png" alt="skill image">
                            </div>
                            <p>Bootstrap5</p>
                        </div>
                        <div class="boxS yet" data-aos="fade-down" data-aos-duration="2000">
                            <div class="imgBox">
                                <img src="./assets/Icons/mongodb-icon.png" alt="skill image">
                            </div>
                            <p>MongoDB</p>
                        </div> -->
        </div>
        <div class="movingSkills">
          <div class="teckSkill">
            <div class="card-header" style="border-bottom: none">
              <h5>Profichinal Skills</h5>
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
            <div class="card-header" style="border-bottom: none">
              <h5>Working On</h5>
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
              <div class="skills" style="width: 0" data-width="2%">0%</div>
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
      </div>
    </div>
    <!-- End Skills  -->

    <!-- Start Education Box -->
    <div class="educationBox mb-3">
      <div class="container">
        <div class="header">
          <h2 id="eduction">
            <ion-icon name="school"></ion-icon> My Education
          </h2>
          <p>
            Education Is Not The Learning Of Facts, But The Training Of The Mind
            To Think.
          </p>
        </div>
        <div class="restCollege">
          <div class="glitchBox" data-aos="fade-down" data-aos-duration="2000">
            <div class="imgBox">
              <img
                src="https://www.elwekalanews.net/UploadCache/libfiles/13/5/600x338o/737.jpg"
                alt="the institute"
              />
            </div>
            <div class="infBox">
              <h5>Bachelor of Business Administration</h5>
              <p>College of engineering, computer science and management</p>
              <span>2021-2025 | Pursuing</span>
            </div>
          </div>
          <div class="imgStudy">
            <img
              src="https://i.pinimg.com/originals/fb/af/44/fbaf443c014bf40b95cfa35121572b25.gif"
              alt="girl study"
            />
          </div>
        </div>
      </div>
    </div>
    <!-- End Education Box -->

    <div class="container my-5">
      <div class="hrPC"></div>
    </div>

    <div class="bordCl"></div>
  </main>

  <!-- main end  -->
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
  spe_color_alot: "text-indigo",
  white_color: "text-white",
});

// Get Icons To Put It On { library } to get from it the icons
import { library } from "@fortawesome/fontawesome-svg-core";
import {
  faPaperPlane,
  faProjectDiagram,
  faUserSecret,
} from "@fortawesome/free-solid-svg-icons";
import {
  faFacebook,
  faGithub,
  faTwitter,
  faLinkedin,
} from "@fortawesome/free-brands-svg-icons";

library.add([faPaperPlane, faProjectDiagram, faUserSecret]);
library.add([faFacebook, faGithub, faTwitter, faLinkedin]);
</script>

<style lang="scss" scoped>
/* start contain of all header of page */
.containAllAbove {
  width: 100%;
  min-height: 80vh;
  background-color: #41464b;
  display: flex;
  flex-direction: row;

  position: relative;
}

/* color mode  */
.colorMode {
  position: absolute;
  left: 6%;
  top: 5%;
  color: var(--for-spesh);
  font-size: 40px;
  border-radius: 50%;
  width: 50px;
  background: #363d44;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 0 12px black, inset 0 0 4px black;
}
.colorMode::before {
  content: "Mode Color";
  position: absolute;
  left: 60px;
  top: 0;
  text-shadow: 0 0 12px;
  color: #363d44;
  transition: 0.4s;
  font-size: 15px;
  width: 100px;
}
.colorMode:hover::before {
  color: var(--for-addition);
}

.colorMode ion-icon {
  filter: drop-shadow(0px 0px 4px black);
  transition: 0.4s;
}
.colorMode:hover ion-icon {
  filter: drop-shadow(0px 0px 20px var(--for-addition));
  color: var(--for-addition);
}

/* Location Button  and  Fire Button */
.containAllAbove .FireBtn {
  right: 10%;
}
.containAllAbove .FireBtn::before {
  content: "Fire";
  position: absolute;
  left: 0;
  top: 40px;
  text-shadow: 0 0 12px;
  color: #363d44;
  transition: 0.4s;
  font-size: 13px;
  width: 100px;
}
.containAllAbove .FireBtn:hover::before {
  color: var(--for-addition);
}

.FireBtn,
.LocationBtn {
  position: absolute;
  right: 5%;
  bottom: 5%;
  color: var(--for-spesh);
  font-size: 40px;
  border-radius: 50%;
  width: 30px;
  background: #363d44;
  height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 0 12px black, inset 0 0 4px black;
}
.FireBtn ion-icon,
.LocationBtn ion-icon {
  filter: drop-shadow(0px 0px 4px black);
  transition: 0.4s;
}
.FireBtn:hover ion-icon,
.LocationBtn:hover ion-icon {
  filter: drop-shadow(0px 0px 20px var(--for-addition));
  color: var(--for-addition);
}

.containAllAbove .LocationBtn::before {
  content: "Location";
  position: absolute;
  left: -10px;
  top: 40px;
  text-shadow: 0 0 12px;
  color: #363d44;
  transition: 0.4s;
  font-size: 13px;
  width: 100px;
}
.containAllAbove .LocationBtn:hover::before {
  color: var(--for-addition);
}

/* up down button with header page */
button.up-to {
  border: none;
  background-color: transparent;
  color: var(--for-spesh);
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  font-size: 25px;
  width: max-content;
  height: max-content;

  top: -25px;
}
/* button.up-to ion-icon {

} */
button.up-to:hover {
  color: var(--for-addition);
  text-shadow: 0 0 12px var(--for-addition);
}

button.down-to {
  border: none;
  background-color: transparent;
  color: var(--for-spesh);
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  font-size: 25px;
  width: max-content;
  height: max-content;

  bottom: -32px;
}
button.down-to:hover {
  color: var(--for-addition);
  text-shadow: 0 0 12px var(--for-addition);
}

/* left headCont start  */
.headCont.left_head {
  right: 2%;
}
.headCont.left_head .contentHeader ul li a {
  font-size: 25px;
}

/* right headCont start  */
.headCont.right_head {
  left: 5%;
}

/* double head contact  */
.headCont {
  padding: 1.3rem;
  position: absolute;
  top: 45%;
  transform: translateY(-50%);
  box-shadow: 0 0 3px black, inset 0 0 12px black;
  border-radius: 5px;
}

.headCont .contentHeader {
  position: relative;
}
.headCont .contentHeader ul {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0;
  padding: 0%;
  gap: 10px;
  height: 250px;
  overflow-y: auto;
}
.headCont .contentHeader ul::-webkit-scrollbar {
  width: 0;
  height: 0;
  background-color: transparent;
}
.headCont .contentHeader ul li {
  list-style: none;
}
.headCont .contentHeader ul li a {
  text-decoration: none;
  font-size: 40px;
  color: var(--for-spesh);
  transition: 0.4s;
}
.headCont .contentHeader ul li a ion-icon {
  filter: drop-shadow(0px 0px 4px rgba(0, 0, 0, 0.678));
  transition: 0.4s;
}
.headCont .contentHeader ul li a:hover ion-icon {
  filter: drop-shadow(0px 0px 20px var(--for-addition));
  color: var(--for-addition);
}

/* header end  */

/* ownImg start  */
.containAllAbove .ownImg {
  z-index: 2;
  position: absolute;
  top: 25%;
  right: 9%;
  width: 345px;
  height: 286px;
}
.containAllAbove .ownImg img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
/* ownImg end  */

/* titling start  */
.containTit {
  background-color: #41464b;
}
.titling {
  z-index: 5;
  padding: 3rem;
  background: #212529;
  clip-path: polygon(
    30% 0,
    100% 0,
    84% 18%,
    84% 70%,
    70% 100%,
    50% 100%,
    0 100%,
    15% 70%,
    15% 32%,
    15% 15%
  );

  color: var(--for-word);
  height: 100%;
}

.titling .infTit {
  position: absolute;
  top: 20%;
  left: 20%;
  max-width: 550px;
  color: var(--for-back);
  background: var(--body);
  padding: 10px;
  border-radius: 5px;
  transition: 0.4s;
  animation: OpacTalkUp 15s infinite;
}
@keyframes OpacTalkUp {
  50%,
  80% {
    opacity: 0;
    visibility: hidden;
  }
  0%,
  47%,
  84% {
    opacity: 1;
    visibility: visible;
  }
}
.titling .infTit::before {
  content: "";
  position: absolute;
  right: -9%;
  bottom: 2%;
  width: 50px;
  height: 50px;
  background: inherit;
  clip-path: polygon(
    23% 54%,
    46% 67%,
    73% 60%,
    100% 37%,
    88% 75%,
    61% 96%,
    36% 96%,
    0 100%,
    0% 35%,
    0 14%
  );
}

.titling .infTit h3 {
  color: var(--for-spesh);
}

.titling .imgTit {
  width: 350px;
  height: 265px;
  position: absolute;
  background: #41464b;
  border-radius: 35%;
  display: flex;
  right: 8%;
  top: 20%;
  justify-content: center;
  align-items: center;
  transition: 0.4s;
  animation: MoveMy 15s infinite;
}
.titling .imgTit img {
  max-width: 95%;
  max-height: 95%;
  border-radius: 35%;
  object-fit: cover;
}
@keyframes MoveMy {
  48% {
    right: 11%;
  }
  50%,
  80% {
    right: -40%;
  }
  82% {
    right: 11%;
  }
  0%,
  47%,
  84% {
    right: 8%;
  }
}

.titling .star {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  animation: animatingStar 8s ease-in-out infinite,
    backgroundMove 16s linear infinite;
}
.titling .star.star1 {
  background: url(./assets/stars/star1.png);
  animation-delay: 0s;
}
.titling .star.star2 {
  background: url(./assets/stars/star2.png);
  animation-delay: -1s;
}
.titling .star.star3 {
  background: url(./assets/stars/star3.png);
  animation-delay: -2s;
}
.titling .star.star4 {
  background: url(./assets/stars/star4.png);
  animation-delay: -3s;
}
.titling .star.star5 {
  background: url(./assets/stars/star5.png);
  animation-delay: -4s;
}
.titling .star.star6 {
  background: url(./assets/stars/star6.png);
  animation-delay: -5s;
}
.titling .star.star7 {
  background: url(./assets/stars/star7.png);
  animation-delay: -6s;
}
.titling .star.star8 {
  background: url(./assets/stars/star8.png);
  animation-delay: -7s;
}

@keyframes animatingStar {
  0%,
  20%,
  40%,
  60%,
  80%,
  100% {
    opacity: 0;
  }
  10%,
  30%,
  50%,
  70%,
  90% {
    opacity: 1;
  }
}
@keyframes backgroundMove {
  0% {
    transform: scale(1);
  }
  100% {
    transform: scale(2);
  }
}

.titling .infTit .hireBtn {
  border: none;
  border-radius: 10px;
  background-color: var(--for-addition);
  color: var(--for-word);
  transition: 0.4s;
}

.titling .infTit .cvBtn {
  border: none;
  border-radius: 10px;
  background-color: var(--for-addition);
  color: var(--for-word);
  transition: 0.4s;
}

.titling .infTit .hireBtn:hover {
  background-color: var(--for-word);
  color: var(--for-addition);
}
.titling .infTit .cvBtn:hover {
  background-color: var(--for-word);
  color: var(--for-addition);
}

.titling .infTit button a {
  text-decoration: none;
  color: var(--for-word);
}
.titling .infTit button:hover a {
  color: var(--for-spesh);
}
.titling .infTit .hireBtn ion-icon {
  display: none;
}

.titling .infTit .cvBtn ion-icon {
  display: none;
}

.titling .infTit .hireBtn.floating {
  border-radius: 50%;
  position: fixed;
  width: 50px;
  left: 35px;
  height: 45px;
  bottom: 20px;
  z-index: 1000;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  box-shadow: 0 0 6px #000;
  animation: ballWater 3s ease-in-out 3s infinite;
}
.titling .infTit .hireBtn.floating a {
  display: none;
}
.titling .infTit .hireBtn.floating ion-icon {
  display: block;
  font-size: 20px;
  text-align: center;
}
.titling .infTit .hireBtn.floating:hover {
  animation: none;
}

.titling .infTit .cvBtn.floating {
  border-radius: 50%;
  position: fixed;
  width: 50px;
  left: 100px;
  height: 45px;
  bottom: 20px;
  z-index: 1000;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  box-shadow: 0 0 6px #000;
  animation: ballWater 3s ease-in-out 3s infinite;
}
.titling .infTit .cvBtn.floating a {
  display: none;
}
.titling .infTit .cvBtn.floating ion-icon {
  display: block;
  font-size: 20px;
  text-align: center;
}

.titling .infTit .cvBtn.floating:hover {
  animation: none;
}

@keyframes ballWater {
  42% {
    bottom: 20px;
  }
  50% {
    bottom: 40px;
  }
  60% {
    bottom: 20px;
  }
  72% {
    bottom: 20px;
  }
  80% {
    bottom: 40px;
  }
  90% {
    bottom: 20px;
  }
  100% {
    bottom: 20px;
  }
}

.titling .infTit button .toolMsg {
  position: absolute;
  bottom: 0px;
  left: -4px;
  background-color: var(--for-spesh);
  padding: 10px;
  transform: translateY(0);
  opacity: 0;
  transition: 0.7s;
  color: var(--for-back);
  border-radius: 4px;
  width: 80px;
}
.titling .infTit .hireBtn.floating:hover .toolMsg {
  opacity: 1;
  transform: translateY(-126%);
}
.titling .infTit .cvBtn.floating:hover .toolMsg {
  opacity: 1;
  transform: translateY(-80%);
}
.titling .infTit button .toolMsg::before {
  content: "";
  position: absolute;
  background-color: var(--for-spesh);
  bottom: -7px;
  left: 38%;
  width: 15px;
  height: 15px;
  transform: rotate(45deg);
}
/* titling end  */

/* part of up to make it full  */
.partUp {
  background-color: #41464b;
  box-shadow: inset 0px -5px 5px 0px black;
  width: 100%;
  z-index: -5;
  height: 100px;
}

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
  box-shadow: inset 0 0 10px 5px;
}
.contentLoc.active {
  transform: scaleY(1);
  visibility: visible;
  opacity: 1;
  position: static;
}

.contentLoc .card-header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.contentLoc .card-header h2 {
  color: var(--for-spesh);
  text-shadow: 0 0 10px black;
  transition: 0.4s;
  animation: LightLoc 5s linear infinite;
}
@keyframes LightLoc {
  0%,
  18%,
  20%,
  50.1%,
  60%,
  65.1%,
  80%,
  90.1%,
  92% {
    color: var(--for-spesh);
    text-shadow: none;
  }
  18.1%,
  20.1%,
  30%,
  50%,
  60.1%,
  65%,
  80.1%,
  90%,
  92.1%,
  100% {
    color: var(--for-addition);
    text-shadow: 0 0 10px var(--for-addition), 0 0 20px var(--for-addition),
      0 0 40px var(--for-addition), 0 0 80px var(--for-addition),
      0 0 160px var(--for-addition);
  }
}

.contentLoc .card-header .closeLocation {
  color: var(--for-spesh);
  filter: drop-shadow(0px 0px 4px black);
  font-size: 30px;
  transition: 0.4s;
}
.contentLoc .card-header .closeLocation:hover {
  color: var(--for-addition);
  filter: drop-shadow(0px 0px 15px var(--for-addition));
}

.contentLoc .card-body {
  height: 500px;
}
.contentLoc .card-body .mapBox {
  padding: 1.3rem;
  box-shadow: 0 0 12px black, inset 0 0 12px black;
  border-radius: 5px;
  height: 100%;
}
.contentLoc .card-body .mapBox iframe {
  width: 100%;
  height: 100%;
  filter: invert(100%);
}

/* End Location Box  */

/* Start About Us  */
.containBoxUs {
  background: url(./assets/imageKav/rog-wallpaper-design-on-behance.gif);
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  background-position: bottom;
  padding: 5rem;
}

.aboutContent {
  background-color: transparent;
  max-height: 400px;
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
}

.aboutContent .imgInfo {
  height: 340px;
}
.aboutContent .imgInfo img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.aboutContent .myInfo {
  color: var(--for-word);
  max-width: 550px;
  border-radius: 5px;
  background: var(--body);
  box-shadow: 0 0 7px rgba(0, 0, 0, 0.4);
  padding: 1rem;
  position: relative;
}

.aboutContent .myInfo .imgGl {
  position: absolute;
  width: 80px;
  height: 80px;
  right: 5%;
  top: -15px;
  border-radius: 50%;
  background: url(https://i0.wp.com/www.lil-ye.com/wp-content/uploads/2020/10/Fantastic.gif?ssl=1&resize=1280%2C1280);
  background-size: 100%;
  border: 5px solid #011f74;
}
.aboutContent .myInfo .imgGl::before {
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
.aboutContent .myInfo .imgGl:hover::before {
  animation: glitchAnim 0.2s linear infinite;
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

.aboutContent .myInfo h3 {
  font-weight: 600;
}
.aboutContent .myInfo p span {
  font-weight: 600;
  font-size: 1.3em;
  color: var(--for-spesh);
}

.aboutContent .myInfo .inf {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}
.aboutContent .myInfo .inf p {
  flex: 1 0 50%;
}
.aboutContent .myInfo .inf span {
  color: var(--for-addition);
  font-size: 13px;
}
/* End About Us  */

/* Start Moving Skills  */
.contentTeckSkills {
  background: transparent;
  width: 100%;
  color: var(--for-word);
}

.staticSkills {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
  padding: 1rem;
  gap: 5rem;
}
.staticSkills .boxS {
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
}
.staticSkills .boxS.yet::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.493);
  z-index: 3;
  border-radius: 50%;
}
.staticSkills .boxS.yet::after {
  content: "Not Yet";
  position: absolute;
  left: 50%;
  top: 50%;
  width: 100%;
  transform: translate(-50%, -50%);
  color: var(--for-addition);
  z-index: 4;
  text-align: center;
  font-weight: 900;
}
.staticSkills .boxS:nth-child(even) {
  animation: FloatingRevBS 1s ease-in-out infinite alternate;
}
.staticSkills .boxS:hover {
  animation-play-state: paused;
  box-shadow: 0 0 30px var(--for-addition);
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
.staticSkills .boxS .imgBox {
  display: block;
  width: 35px;
  height: 35px;
}
.staticSkills .boxS .imgBox img {
  object-fit: contain;
  width: 100%;
  height: 100%;
}
.staticSkills .boxS p {
  color: #dc3535;
  font-weight: 600;
  font-size: 13px;
}

.movingSkills {
  position: relative;
  transition: 1s;
}

.movingSkills .teckSkill {
  transform-style: preserve-3d;
  padding: 1.5rem;
}
.movingSkills .teckSkill h5 {
  color: var(--for-spesh);
  font-weight: 600;
  font-family: var(--font-bold);
}
.movingSkills .teckSkill p {
  padding-left: 6rem;
  margin: 0;
  color: var(--for-word);
}

.containerTeckSkill {
  width: 100%;
  background-color: #e1e1e1;
  height: auto;
  padding: 10px;
}

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

.movingSkills .proSkills {
  transform-style: preserve-3d;
  padding: 1.5rem;
}
.movingSkills .proSkills h3 {
  text-align: center;
  color: var(--for-spesh);
  font-weight: 600;
  font-family: var(--font-bold);
}

/* here contain circles */
/* .movingSkills .proSkills .containCircles {
} */

/* .skill {
    width: 95px;
    height: 90px;
    position: relative;
}
.outher {
    width: 95px;
    height: 90px;
    border-radius: 50%;
    padding: 14px;
}
.inner {
    width: 65px;
    height: 60px;
    border-radius: 50%;
    box-shadow: inset 4px 4px 6px -1px rgba(0, 0, 0, 0.2),
                inset -4px -4px 6px -1px rgba(255, 255, 255, 0.7),
                1px 2px 0px rgb(255 255 255),
                0.5px 0.5px 0px rgba(0, 0, 0, 0.15),
                0px 12px 10px -10px rgba(0, 0, 0, 0.5);
    display: flex;
    align-items: center;
    justify-content: center;
}
#number {
    color: var(--for-word);
    font-weight: 600;
}
#CirOne {
    fill: none;
    stroke: #456fe5;
    stroke-width: 20px;
    stroke-dasharray: 472;
    stroke-dashoffset: 472;
    transition: 1.4s;
}
#svgCir {
    position: absolute;
    top: 0;
    left: 0;
}


.nameCir {
    text-align: center;
    font-weight: 600;
    color: var(--for-spesh);
}

#CirTwo {
    fill: none;
    stroke: #456fe5;
    stroke-width: 20px;
    stroke-dasharray: 472;
    stroke-dashoffset: 472;
    transition: 1.4s;
}


#CirThre {
    fill: none;
    stroke: #456fe5;
    stroke-width: 20px;
    stroke-dasharray: 472;
    stroke-dashoffset: 472;
    transition: 1.4s;
}

#CirFour {
    fill: none;
    stroke: #456fe5;
    stroke-width: 20px;
    stroke-dasharray: 472;
    stroke-dashoffset: 472;
    transition: 1.4s;
} */
/* the Cycles End  */

/* End Moving Skills  */

/* Start Education Box */
.educationBox {
  background: #41464b;
  width: 100%;
  min-height: 300px;
  padding: 2rem;
  box-shadow: inset 0 0 8px;
}
.educationBox .header p {
  color: var(--for-spesh);
  text-align: center;
}

.educationBox .restCollege {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.educationBox .restCollege .glitchBox {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  background: var(--body);
  margin: 1rem;
  display: flex;
  align-items: center;
  transition: 0.4s;
  border-radius: 5px;
}
.educationBox .restCollege .glitchBox:hover {
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.7);
}

.educationBox .restCollege .glitchBox .imgBox {
  width: 250px;
  height: 100%;
  border-radius: 5px;
}
.educationBox .restCollege .glitchBox .imgBox img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.educationBox .restCollege .glitchBox .infBox {
  padding: 1rem;
  flex: 1 1;
  font-weight: 600;
}
.educationBox .restCollege .glitchBox .infBox h5 {
  color: #dc3535;
}
.educationBox .restCollege .glitchBox .infBox p {
  color: var(--for-word);
  font-weight: 400;
}
.educationBox .restCollege .glitchBox .infBox span {
  color: #237e51;
}

.educationBox .restCollege .imgStudy {
  flex: 1 1;
  border-radius: 7px;
}
.educationBox .restCollege .imgStudy img {
  object-fit: contain;
  width: 100%;
  height: 100%;
  border-radius: 7px;
}
/* End Education Box */

.hrPC {
  width: 100%;
  position: relative;
  background-color: #000000;
  height: 1px;
}
.hrPC::before {
  content: "";
  background: url(./assets/Icons/stars-icon.png);
  position: absolute;
  background-repeat: no-repeat;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  width: 40px;
  height: 20px;
  background-size: contain;
  z-index: 4;
}
.hrPC::after {
  content: "";
  background: var(--body);
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  width: 50px;
  height: 50px;
  z-index: 2;
}
</style>