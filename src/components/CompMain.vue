<script>
export default {
    name: 'CompMain',
    data() {
        return {
            datesList: [
                {
                    text: '17/08/2020 GEM FESTIVAL 2020 ANAKALIA, GEORGIA'
                },
                {
                    text: '24/09/2020 GROOVEFEST DOMINICAL REPUBLIC'
                },
                {
                    text: '31/10/2020 OASIS FESTVAL 2020 MARRAKECH, MOROCCO'
                },
                {
                    text: '07/11/2020 MOGA FESTIVAL - ESSAOURIA, MOROCCO'
                },
                {
                    text: '10/12/2020 ENVISION FESTIVAL - UVITA, COSTA RICA'
                },

            ]
        }
    }
}
</script>
<template>
    <main>
        <section class="paragraph-section">
            <div class="container">
                <div class="row">
                    <div class="col-6 m-auto pt-3">
                        <h2 class="paragraph-title pb-4">Music is LIfe</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                            laudantium,
                            dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                            ullam.

                        </p>
                    </div>
                </div>
            </div>
        </section>
        <section class="main-section">
            <div class="container">
                <div class="row">
                    <div class="col-6 m-auto pt-3 mb-5">
                        <h2 class="paragraph-title pb-4">Latest Band News</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                            laudantium,
                            dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                            ullam.
                        </p>
                    </div>
                </div>
                <div class="cards-wrapper col-10 d-flex m-auto justify-content-center">

                    <!-- sezione sinistra delle card  -->

                    <div class="col-6 d-flex flex-wrap left-side me-3">
                        <div class="card horizontal-card mb-3">

                        </div>

                        <div class="card  vertical-card mb-3">

                        </div>

                        <div class="card  vertical-card mb-3">

                        </div>
                        <div class="card horizontal-card">

                        </div>
                    </div>

                    <!-- sezione destra delle carte  -->

                    <div class="col-3 right-side">
                        <div class=" card vertical-card">

                        </div>
                        <div class="card vertical-card">

                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- divider -->

        <section class="divider">
            <div class="container-fluid">
                <div class="row align-items-center">
                    <div class="col-4 m-auto">
                        <a href="#" class="text-white">VIEW ALL LATEST NEWS</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- second jumbo -->

        <section class="jumbo">
            <div class="container">
                <div class="row">
                    <div class="col-6 m-auto text-center intervew-wrapper">
                        <p class="intervew">"I just listened to it and said to myself, "Man, I really love this album."
                            Still, today, it
                            just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're
                            good. And they're inventive. I haven't heard anything this year that's as inventive. I don't
                            really expect to."
                        </p>
                        <button>
                            <img src="../assets/images/band_interview_play_icon.png" alt="#">
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- date-section -->
        <section class="date-section">
            <div class="container">
                <div class="row">
                    <div class="col-6 m-auto pt-3">
                        <h2 class="paragraph-title pb-4">Live Dates</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                            laudantium,
                            dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                            ullam.
                        </p>
                    </div>
                </div>
                <div class="col-10 m-auto">
                    <div class="date-list">
                        <ul class="mt-4">
                            <li v-for="dateElement in datesList">
                                + {{ dateElement.text }}
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

    </main>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

.paragraph-section {
    height: 225px;
    background-color: $bg-color-small-section;
}

.main-section {
    background-color: $bg-principal-section;
}

.date-section {
    background-color: $bg-principal-section;

    .date-list {
        color: $li-date-color;
        text-align: left;

        ul {
            list-style-type: none;

            li {
                background-color: $bg-color-small-section;
                padding: 0.5rem;
                margin-bottom: 0.6rem;
            }
        }
    }
}

.paragraph-title {
    border-bottom: 1px solid $words;
}


.cards-wrapper {
    padding-bottom: 4rem;
}

.horizontal-card {
    width: 100%;
    height: 180px;
    background-color: $bg-color-small-section;
}

.vertical-card {
    height: 300px;
    width: calc((100% / 2) - 0.5rem);
    margin-right: 0.5rem;
    background-color: $bg-color-small-section;
}

.right-side {
    .vertical-card {
        width: 100%;
        height: calc((100% / 2) - 1rem);
        margin-bottom: 0.5rem;
    }
}

.divider {
    background-color: $divider-color;
}

.jumbo {
    height: 80vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url("../assets/images/home-testimonial-parallax.jpg");
    background-position: center;
    background-size: cover;

    .intervew {
        color: white;
        font-size: 1rem;
        font-style: italic;
    }

    button {
        background: none;
        border: none;

        img {
            width: 60px;
        }
    }
}
</style>