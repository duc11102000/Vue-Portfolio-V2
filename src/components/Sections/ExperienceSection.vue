<template>
    <div id="experience">
        <section>
            <p class="section__text__p1">Explore My</p>
            <h1 class="title">Experience</h1>
            <div class="experience-details-container">
                <div class="about-containers">
                    <div class="details-container">
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
                    <div class="details-container">
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
    </div>
</template>

<style scoped lang="scss">
#experience {
    background: #005B91;

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


}
</style>