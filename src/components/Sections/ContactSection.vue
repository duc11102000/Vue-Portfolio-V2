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
        </section>
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
    
    section {
        position: relative;
        display: flex;
        justify-content: center;
        flex-direction: column;
        padding: 9rem 0;

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



}
</style>