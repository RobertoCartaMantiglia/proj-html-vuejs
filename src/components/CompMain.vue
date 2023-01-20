
<script>
import VerticalCardRight from './VerticalCardRight.vue';
import DividerLink from './DividerLink.vue';
import CompDates from './CompDates.vue';
export default {
    name: 'CompMain',
    components: {
        VerticalCardRight,
        DividerLink,
        CompDates,
    },

}
</script>
<template>
    <main>
        <section class="paragraph-section">
            <div class="container">
                <div class="upper-separate m-auto"></div>
                <div class="row">
                    <div class="col-6 m-auto pt-5">
                        <h2 class="paragraph-title">Music is LIfe</h2>
                        <div class="paragraph-underline m-auto my-4"></div>
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
                    <div class="col-6 m-auto pt-5 mb-5">
                        <h2>Latest Band News</h2>
                        <div class="paragraph-underline m-auto my-4"></div>
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
                        <div class="card horizontal-card-wrap mb-3">
                            <div class="horizon-card">
                                <img src="../assets/images/blog_music_techo-600x300.jpg" alt="#">
                                <div class="card-info p-2">
                                    <h4 class="pt-3">Technology and Music</h4>
                                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa
                                        consequuntur non debitis
                                    </p>
                                </div>
                            </div>
                        </div>

                        <div class="card vertical-card-wrap mb-3">
                            <div class="vertical-card">
                                <img src="../assets/images/blog-post3-600x900.jpg" alt="#">
                                <div class="card-info p-2">
                                    <h4 class="pt-3">While my Guitar gently weeps</h4>
                                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa
                                        consequuntur non debitis
                                    </p>
                                </div>
                            </div>
                        </div>
                        <div class="card vertical-card-wrap mb-3">
                            <div class="vertical-card">
                                <img src="../assets/images/blog-post4-600x900.jpg" alt="#">
                                <div class="card-info p-2">
                                    <h4 class="pt-3">It just sounds better</h4>
                                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa
                                        consequuntur non debitis
                                    </p>
                                </div>
                            </div>
                        </div>
                        <div class="card horizontal-card-wrap">
                            <div class="horizon-card">
                                <img src="../assets/images/blog_flavor_rock-600x300.jpg" alt="#">
                                <div class="card-info p-2">
                                    <h4 class="pt-3">The flavour of Rock</h4>
                                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa
                                        consequuntur non debitis
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- sezione destra delle carte  -->

                    <div class="col-3 right-side">
                        <VerticalCardRight />
                    </div>
                </div>
            </div>
        </section>

        <!--primo divider -->

        <section class="divider-section">
            <DividerLink />
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
        <section class="date-section pb-5">
            <CompDates />
        </section>

        <!--secondo  divider -->

        <section class="divider">
            <div class="container-fluid">
                <div class="row align-items-center">
                    <div class="col-4 m-auto">
                        <a href="#">VIEW ALL LIVE DATES</a>
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

}

.upper-separate {
    width: 280px;
    border: 4px solid $divider-color;
}

.paragraph-underline {
    width: 180px;
    border: 1px solid $background-social;
}

.cards-wrapper {
    padding-bottom: 4rem;
}

.horizontal-card-wrap {
    width: 100%;
    height: 300px;
    background-color: $bg-color-small-section;

    .horizon-card {
        width: 100%;
        height: 100%;
        text-align: left;

        img {
            width: 100%;
            height: 60%;
        }

        h4 {
            color: $card-title;
            font-size: 0.9rem;
            font-weight: bold;
        }
    }

    .horizon-card:hover {
        img {
            opacity: 0.8;
            transition: 0.5s ease-in-out;
        }
    }
}

.vertical-card-wrap {
    height: 440px;
    display: flex;
    width: calc((100% / 2) - 0.5rem);
    margin-right: 0.5rem;
    background-color: $bg-color-small-section;

    .vertical-card {
        width: 100%;
        height: 100%;
        text-align: left;

        img {
            width: 100%;
            height: 70%;
        }

        h4 {
            color: $card-title;
            font-size: 0.9rem;
            font-weight: bold;
        }
    }

    .vertical-card:hover {
        img {
            opacity: 0.8;
            transition: 0.5s ease-in-out;
        }
    }
}

// DIVIDER 
.divider {
    background-color: $divider-color;
    transition: background-color 0.5s;

    a {
        color: white;
        font-size: 0.9rem;
    }
}

.divider:hover {
    background-color: white;

    a {
        color: black;
    }
}

// JUMBO 
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
        transition: 0.3s;

        img {
            width: 60px;
        }
    }

    button:hover {
        transform: scale(1.2);
    }
}
</style>