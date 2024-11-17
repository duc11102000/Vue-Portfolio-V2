<!-- {{ projectData.projectsArray }} -->
<!-- ảnh thì dùng trang https://www.base64-image.de/ -->
<template>
  <div id="projects">
    <section>
      <p class="section__text__p1" data-aos="fade-down">Browse My Recent</p>
      <h1 class="title" data-aos="fade-down">Projects</h1>
      <swiper
        :modules="modules"
        :slides-per-view="swiperOptions.slidesPerView"
        :space-between="swiperOptions.spaceBetween"
        :autoplay="{
          delay: 2500,
          disableOnInteraction: false,
        }"
        :breakpoints="swiperOptions.breakpoints"
        class="projects-details-container"
      >
        <swiper-slide
          v-for="(items, index) in projectData.projectsArray"
          :key="items"
        >
          <div class="details-container" data-aos="flip-up">
            <div class="article-container">
              <img
                :src="projectData.projectsArray[index].Image"
                alt="Project 1"
                class="project-img w-[150px]"
              />
            </div>
            <h2 class="experience-sub-title project-title">
              {{ projectData.projectsArray[index].Title }}
            </h2>
            <p>
              {{ projectData.projectsArray[index].About }}
            </p>
            <div class="btn-container">
              <a
                class="project-btn"
                :href="projectData.projectsArray[index].Link1"
                target="_blank"
              >
                Landing Page
              </a>
              <a
                class="project-btn"
                :href="projectData.projectsArray[index].Link2"
                target="_blank"
              >
                DApp
              </a>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </section>
    <div class="bubble bubble-1"></div>
    <div class="bubble bubble-2"></div>
    <div class="wave">
      <svg
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path
          d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
          class="shape-fill"
        ></path>
      </svg>
    </div>
  </div>
</template>

<script setup>
import jsonData from "../../../projects.json";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay } from "swiper/modules";
import AOS from "aos";
import "swiper/css";
import "swiper/css/autoplay";
import "aos/dist/aos.css";
import { ref, onMounted } from "vue";

const projectData = jsonData;

const modules = [Autoplay];
const swiperOptions = ref({
  // Common options
  slidesPerView: 3,
  spaceBetween: 50,
  // Breakpoints
  breakpoints: {
    // When window width is >= 768px
    990: {
      slidesPerView: 3,
      spaceBetween: 30,
    },

    319: {
      slidesPerView: 1,
      spaceBetween: 30,
    },
    // When window width is >= 1024px
  },
});

onMounted(() => {
  AOS.init();
});
</script>

<style scoped lang="scss">
#projects {
  background: #3f9dd5;
  position: relative;
  z-index: 999;

  section {
    position: relative;
    padding: 5rem 0;
    // height: 100vh;

    .title {
      text-align: center;
      font-size: 4rem;
      font-weight: 700;
      color: #fff;
    }

    .section__text__p1 {
      font-size: 22px;
      text-align: center;
      color: #fff;
      margin-top: 3rem;
    }

    .projects-details-container {
      margin-top: 40px;
      padding: 2rem 0;
    }

    .details-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;
      gap: 15px;
      padding: 1.5rem;
      background: white;
      border-radius: 2rem;
      text-align: center;
      height: 500px;
      cursor: pointer;
      box-shadow: rgba(0, 0, 0, 0.3) 10px 12px 12px;
    }

    .details-container p {
      text-align: left;
    }

    // .project-img {
    //   width: 90%;
    // }

    .project-title {
      font-size: 22px;
      font-weight: 600;
      color: #005b91;
    }

    .btn-container {
      display: flex;
      justify-content: center;
      gap: 1rem;
    }

    .project-btn {
      text-decoration: none;
      border: 2px solid #005b91;
      font-weight: 600;
      transition: all 300ms ease;
      padding: 9px 10px;
      width: 160px;
      border-radius: 2rem;
      color: #005b91;
      background: none;

      &:hover {
        background: #005b91;
        color: white;
      }
    }
  }

  .bubble {
    position: absolute;
    z-index: -999;
    background: #206690;
  }

  .bubble-1 {
    top: 50%;
    left: 15px;
    border-radius: 100%;
    width: 400px;
    height: 400px;
  }

  .bubble-2 {
    top: 30%;
    right: 15px;
    border-radius: 100%;
    width: 300px;
    height: 300px;
  }

  .wave {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
  }

  .wave svg {
    position: relative;
    display: block;
    width: calc(117% + 1.3px);
    height: 271px;
  }

  .wave .shape-fill {
    fill: #005b91;
  }
}
</style>
