<template>
    <div id="profile">
        <section>
            <div class="section__pic-container" data-aos="fade-down">
                <img src="../../assets/images/profile.jpg" alt="picture" />
            </div>
            <div class="section__text" data-aos="fade-up">
                <p class="section__text__p1">Hello, I'm</p>
                <h1 class="title">Nguyễn Hữu Đức</h1>
                <p class="section__text__p2">Frontend Developer</p>
                <div class="btn-container">
                    <a href="https://drive.google.com/file/d/1a7JBh8SwpJwnbwWddTO_wUr-AVw5p5BW/view?usp=drive_link"
                        target="_blank" class="btn btn-color-2">
                        Download CV
                    </a>
                    <a class="btn btn-color-1" onclick="location.href='./#contact'">
                        Contact Info
                    </a>
                </div>
                <div id="socials-container">
                    <a class="github w-[40px]" href="https://github.com/duc11102000" target="_blank">
                        <img src="../../assets/images/github.png" alt="My Github profile" class="icon" />
                    </a>
                </div>
            </div>
        </section>
        <div class="bubble bubble-1" data-aos="fade-up"></div>
        <div class="bubble bubble-2" data-aos="fade-up"></div>
        <div class="bubble bubble-3" data-aos="fade-up"></div>
        <div class="bubble bubble-4" data-aos="fade-up"></div>
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
#profile {
    background: #3F9DD5;
    position: relative;
    z-index: 999;

    .flip {
        transform: rotate(180deg);
    }

    section {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 5rem;
        height: 83vh;
        width: 90%;
        margin: 0 auto;

        .title {
            text-align: center;
            font-size: 3rem;
            font-weight: 700;
            color: #fff;
        }

        p {
            color: #fff;
            margin: 0;
            padding: 0;
        }

        a {
            text-decoration: none;
            color: #fff;
        }

        .section__pic-container {
            width: 315px;

            img {
                border-radius: 2rem;
            }
        }

        .section__text {
            align-self: center;
            text-align: center;

            p {
                font-weight: 600;
            }
        }


        .section__text__p1 {
            text-align: center;
        }

        .section__text__p2 {
            font-size: 1.75rem;
            margin-bottom: 1rem;
            color: #002f4b;
        }

        #socials-container {
            display: flex;
            justify-content: center;
            margin-top: 1rem;
            gap: 1rem;
        }

        /* --------------BUTTONS------------------ */

        .btn-container {
            display: flex;
            justify-content: center;
            gap: 1rem;
        }

        .btn {
            font-weight: 600;
            transition: all 300ms ease;
            padding: 1rem 2rem;
            border-radius: 2rem;
            background: #002f4b;
            cursor: pointer;

            &:hover {
                background: #005b91;
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


    @media (max-width: 991px) {
        section {
            flex-direction: column;
            height: 100%;
            padding: 15px;
            gap: 2rem;
        }
    }
}
</style>