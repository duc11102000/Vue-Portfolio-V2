<template>
    <div id="experience">
        <section>
            <p class="section__text__p1" data-aos="fade-down">Explore My</p>
            <h1 class="title" data-aos="fade-down">Experience</h1>
            <div class="experience-details-container">
                <div class="about-containers">
                    <div class="details-container" data-aos="flip-left">
                        <h2 class="experience-sub-title">Front-end Development</h2>
                        <div class="article-container">
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>HTML</h3>
                                    <p>Intermediate</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>CSS</h3>
                                    <p>Intermediate</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>SASS</h3>
                                    <p>Experienced</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>JavaScript</h3>
                                    <p>Intermediate</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>TypeScript</h3>
                                    <p>Basic</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>Boostrap</h3>
                                    <p>Experienced</p>
                                </div>
                            </article>
                        </div>
                    </div>
                    <div class="details-container" data-aos="flip-right">
                        <h2 class="experience-sub-title">Front-end Development</h2>
                        <div class="article-container">
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>Vue JS</h3>
                                    <p>Intermediate</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>React JS</h3>
                                    <p>Basic</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>Node JS</h3>
                                    <p>Basic</p>
                                </div>
                            </article>
                            <article>
                                <img src="../../assets/images/checkmark.png" alt="Experience icon" class="icon" />
                                <div>
                                    <h3>Git</h3>
                                    <p>Intermediate</p>
                                </div>
                            </article>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <div class="bubble bubble-1" data-aos="zoom-in-up"></div>
        <div class="bubble bubble-2" data-aos="zoom-in-up"></div>
        <div class="bubble bubble-3" data-aos="zoom-in-up"></div>
        <div class="bubble bubble-4" data-aos="zoom-in-up"></div>
        <div class="bubble bubble-5" data-aos="zoom-in-up"></div>
        <div class="bubble bubble-6" data-aos="zoom-in-up"></div>
        <div class="bubble bubble-7" data-aos="zoom-in-up"></div>
        <div class="wave">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120"
                preserveAspectRatio="none">
                <path
                    d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
                    class="shape-fill"></path>
            </svg>
        </div>
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
#experience {
    background: #005B91;
    position: relative;
    z-index: 999;
    // background-image: url('@/assets/images/bg-code.svg');
    // background-repeat: no-repeat;   

    section {
        position: relative;
        margin-top: 100px;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;

        .title {
            text-align: center;
            font-size: 4rem;
            font-weight: 700;
            color: #fff;
        }

        h3,
        p {
            margin-top: 0;
            margin-bottom: 0;
        }

        p {
            color: rgb(85, 85, 85);
        }

        .section__text__p1 {
            color: #fff;
            text-align: center;
            font-size: 22px;
        }

        .experience-sub-title {
            color: rgb(85, 85, 85);
            font-weight: 600;
            font-size: 1.75rem;
            margin-bottom: 2rem;
        }

        .experience-details-container {
            display: flex;
            justify-content: center;
            flex-direction: column;
        }

        .article-container {
            display: flex;
            text-align: initial;
            flex-wrap: wrap;
            flex-direction: row;
            gap: 2.5rem;
            justify-content: space-around;
        }

        .about-containers {
            display: flex;
            gap: 2rem;
            margin-bottom: 2rem;
            margin-top: 2rem;
        }

        .details-container {
            padding: 1.5rem;
            flex: 1;
            background: white;
            border-radius: 2rem;
            text-align: center;

            h2 {
                color: #3f9dd5;
            }

            article {
                display: flex;
                width: 10rem;
                gap: 0.5rem;

                h3,
                p {
                    font-size: 18px;
                }

                div {
                    margin-left: 10px;
                }

                .icon {
                    cursor: default;
                }

                img {
                    height: 2rem;
                }
            }
        }

    }

    .bubble {
        position: absolute;
        z-index: -999;
    }

    .bubble-1 {
        top: 50%;
        left: 15px;
        border-radius: 100%;
        width: 225px;
        height: 225px;
        background: #2883b9;
    }

    .bubble-2 {
        top: 30%;
        right: 15px;
        border-radius: 100%;
        width: 300px;
        height: 300px;
        background: #2883b9;
    }

    .bubble-3 {
        top: 5%;
        left: 100px;
        border-radius: 100%;
        width: 150px;
        height: 150px;
        background: #2883b9;
    }


    .bubble-4 {
        top: 5%;
        right: 30%;
        border-radius: 100%;
        width: 150px;
        height: 150px;
        background: #2883b9;
    }

    .bubble-5 {
        top: 50%;
        right: 35%;
        border-radius: 100%;
        width: 300px;
        height: 300px;
        background: #2883b9;
    }

    .wave {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        overflow: hidden;
        line-height: 0;

        svg {
            position: relative;
            display: block;
            width: calc(143% + 1.3px);
            height: 112px;
        }

        .shape-fill {
            fill: #FFFFFF;
        }
    }
}
</style>