<template>
    <div id="about" class="bubble">
        <section >
            <p class="section__text__p1" data-aos="fade-down">Get To Know More</p>
            <h1 class="title" data-aos="fade-down">About Me</h1>
            <div class="section-container">
                <div class="about-details-container">
                    <div class="about-containers">
                        <div class="details-container" data-aos="flip-left">
                            <img src="../../assets/images/experience.png" alt="Experience icon" class="icon" />
                            <h3>Experience</h3>
                            <p>6+ months <br />Frontend Development</p>
                        </div>
                        <div class="details-container" data-aos="flip-right">
                            <img src="../../assets/images/education.png" alt="Education icon" class="icon" />
                            <h3>Education</h3>
                            <p>HUTECH University</p>
                        </div>
                    </div>
                    <div class="text-container" data-aos="fade-up">
                        <p>
                            Hi, I'm <strong>Nguyễn Hữu Đức</strong>, i'm from the
                            <strong>HUTECH University</strong>, major in
                            <strong>Software Engineer</strong>. I have a profound
                            passion for <strong>Front-End Technology</strong>, and I love to create beautiful
                            and performant products with delightful user experiences.
                            Proficient in <strong>HTML</strong>, <strong>CSS</strong>, and
                            <strong>Javascript</strong>, along with expertise in the
                            <strong>Vue.JS</strong> framework, i am looking forward to be a
                            professional <strong>Front-end Developer</strong> in a highly productive work
                            environment.
                        </p>
                    </div>
                </div>
            </div>
            <div class="bubble bubble-1" data-aos="zoom-in"></div>
            <div class="bubble bubble-2" data-aos="zoom-in"></div>
            <div class="bubble bubble-3" data-aos="zoom-in"></div>
            <div class="bubble bubble-4" data-aos="zoom-in"></div>
            <div class="bubble bubble-5" data-aos="zoom-in"></div>
        </section>

    </div>
</template>

<script setup>
import AOS from 'aos';
import 'aos/dist/aos.css';
import { ref, onMounted } from 'vue'

onMounted(() => {
    AOS.init();
})
</script>

<style scoped lang="scss">
#about {
    background: #3F9DD5;
    position: relative;
    z-index: 999;

    section {
        position: relative;
        z-index: 1;

        p {
            color: #002f4b;
            font-size: 22px;
            font-weight: 500;
            line-height: 40px;
        }

        .title {
            text-align: center;
            font-size: 4rem;
            font-weight: 700;
            color: #3f9dd5;
        }

        .about-containers {
            gap: 2rem;
            margin-bottom: 2rem;
            margin-top: 2rem;
        }

        .about-details-container {
            width: 800px;
            margin: 0 auto;
            justify-content: center;
            flex-direction: column;

            .about-containers,
            .about-details-container {
                display: flex;
            }

            .text-container {
                strong {
                    color: #3f9dd5;
                }
            }
        }

        .about-pic {
            border-radius: 2rem;
        }

        .arrow {
            position: absolute;
            right: -5rem;
            bottom: 2.5rem;
        }

        .details-container {
            padding: 1.5rem;
            background: white;
            border-radius: 2rem;
            flex: 1;
            border: 0.1rem solid #002f4b;
            text-align: center;

            h3 {
                font-size: 18px;
                font-weight: 600;
                margin: 15px 0;
            }

            img {
                width: 2rem;
                margin: 0 auto;
            }
        }

        .section-container {
            gap: 4rem;
            height: 80%;
        }

        .section__pic-container {
            height: 400px;
            width: 400px;
            margin: auto 0;
        }

        .section__text__p1 {
            text-align: center;
            margin-top: 3rem;
        }

        .section__text__p2 {
            font-size: 1.75rem;
            margin-bottom: 1rem;
            color: rgb(85, 85, 85);
        }

        @media screen and (max-width: 1400px) {
            .about-containers {
                flex-wrap: wrap;
            }
        }

        .bubble {
            position: absolute;
            z-index: -999;
            overflow: hidden;

        }

        .bubble-1 {
            background: #dceaf3;
            top: 50%;
            left: 15px;
            border-radius: 100%;
            width: 250px;
            height: 250px;
        }

        .bubble-2 {
            background: #dceaf3;
            top: 30%;
            right: 15px;
            border-radius: 100%;
            width: 150px;
            height: 150px;
        }

        .bubble-3 {
            background: #dceaf3;
            top: 30%;
            right: 50%;
            border-radius: 100%;
            width: 100px;
            height: 100px;
        }

        .bubble-4 {
            background: #dceaf3;
            top: 70%;
            right: 5%;
            border-radius: 100%;
            width: 100px;
            height: 100px;
        }

        .bubble-5 {
            background: #dceaf3;
            top: 70%;
            right: 35%;
            border-radius: 100%;
            width: 300px;
            height: 300px;
        }
    }


}

#about::before {
    content: '';
    border-top-left-radius: 85% 100%;
    border-top-right-radius: 85% 100%;
    position: absolute;
    bottom: 0;
    z-index: 1;
    width: 100%;
    background-color: #fff;
    height: 100%;
}
</style>