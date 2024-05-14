<template>
    <div id="profile">
        <section>
            <div class="section__pic-container">
                <img src="../../assets/images/profile2.png" alt="picture" />
            </div>
            <div class="section__text">
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
    </div>
</template>

<style scoped lang="scss">
#profile {
    background: #3F9DD5;

    section {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 5rem;
        height: 83vh;

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

}
</style>