<!-- {{ projectData.projectsArray }} -->
<!-- ảnh thì dùng trang https://www.base64-image.de/ -->
<template>
    <div id="projects">
        <section>
            <p class="section__text__p1">Browse My Recent</p>
            <h1 class="title">Projects</h1>
            <swiper :modules="modules" :slides-per-view="swiperOptions.slidesPerView"
                :space-between="swiperOptions.spaceBetween" :autoplay="{
                    delay: 2500,
                    disableOnInteraction: false,
                }" :breakpoints="swiperOptions.breakpoints" class="projects-details-container">
                <swiper-slide v-for="(items, index) in projectData.projectsArray" :key="items">
                    <div class="details-container">
                        <div class="article-container">
                            <img :src="projectData.projectsArray[index].Image" alt="Project 1" class="project-img" />
                        </div>
                        <h2 class="experience-sub-title project-title">
                            {{ projectData.projectsArray[index].Title }}
                        </h2>
                        <p>
                            {{ projectData.projectsArray[index].About }}
                        </p>
                        <div class="btn-container">
                            <a class="project-btn" :href="projectData.projectsArray[index].Link1" target="_blank">
                                Github </a>
                            <a class="project-btn" :href="projectData.projectsArray[index].Link2" target="_blank"> Live
                                Demo </a>
                        </div>
                    </div>
                </swiper-slide>
            </swiper>
        </section>
    </div>
</template>

<script setup>
import jsonData from '../../../projects.json'
import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay } from "swiper/modules";
import "swiper/css";
import "swiper/css/autoplay";

const projectData = jsonData

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
</script>

<style scoped lang="scss">
#projects {
    background: #3F9DD5;

    section {
        position: relative;
        padding: 5rem 0;
        height: 100vh;

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
        }

        .projects-details-container {
            margin-top: 40px;
            padding: 2rem 0;
        }

        .details-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 15px;
            padding: 1.5rem;
            background: white;
            border-radius: 2rem;
            text-align: center;
            height: 400px;
            cursor: pointer;
            box-shadow: rgba(0, 0, 0, 0.3) 10px 12px 12px;
            ;
        }

        .details-container p {
            text-align: left;
        }

        .project-img {
            border-radius: 2rem;
            width: 90%;
            height: 90%;
        }

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
            padding: 1rem;
            width: 8rem;
            border-radius: 2rem;
            color: #005b91;
            background: none;

            &:hover {
                background: #005b91;
                color: white;
            }
        }
    }



}
</style>