<template>
    <div id="contact">
        <section>
            <p class="section__text__p1">Get in Touch</p>
            <h1 class="title">Contact Me</h1>
            <div class="contact-info-upper-container">
                <div class="contact-info-container">
                    <img src="../../assets/images/email.png" alt="email icon" class="icon contact-icon email-icon" />
                    <p>
                        <a href="mailto:duc11102000@gmail.com">duc11102000@gmail.com</a>
                    </p>
                </div>
                <div class="contact-info-container">
                    <img src="../../assets/images/phone2.png" alt="phone icon" class="icon contact-icon" />
                    <p><a href="tel:0968765936">0968765936</a></p>
                </div>
            </div>
            <!-- <a class="backtotop" @click="scrollToTop"><img src="../../assets/images/arrow.png" alt="Arrow icon"
                    class="icon arrow" /></a> -->
            <!-- <div class="spacer layer-1">
            </div> -->
        </section>
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
const scrollToTop = () => {
    window.scrollTo(0, 0);
}
</script>

<style scoped lang="scss">
#contact {
    background: #005B91;
    position: relative;

    section {
        position: relative;
        display: flex;
        justify-content: center;
        flex-direction: column;
        padding: 5rem 0;

        a {
            color: #005b91;
            text-decoration: none;
            text-decoration-color: #005b91;
            transition: all 300ms ease;
            font-weight: 500;

            &:hover {
                text-decoration: underline;
                text-underline-offset: 1rem;
            }
        }

        .title {
            text-align: center;
            font-size: 4rem;
            font-weight: 700;
            color: #fff;
        }

        .section__text__p1 {
            text-align: center;
            color: #fff;
            font-size: 22px;
        }

        .contact-info-upper-container {
            display: flex;
            justify-content: center;
            border-radius: 2rem;
            margin: 2rem auto;
            padding: 0.5rem;
            background: #fff;
        }

        .contact-info-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
            margin: 1rem;

            p {
                font-size: larger;
            }

            .email-icon,
            .contact-icon {
                height: 2.5rem;
            }
        }

        .backtotop {
            position: absolute;
            right: 0;
            bottom: 0;

            a {
                cursor: pointer;
            }

            img {
                height: 2rem;
                transform: rotate(180deg);
            }
        }
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
            width: calc(133% + 1.3px);
            height: 79px;
        }

        .shape-fill {
            fill: #3F9DD5;
        }
    }
}
</style>