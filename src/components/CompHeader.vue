
<script>
import NavBar from './NavBar.vue';
export default {
    name: 'CompHeader',
    components: {
        NavBar,
    },
}
</script>
<template>
    <header class="jumbo">
        <section>
            <div class="container-fluid">
                <div class="row">
                    <div class="col-12 d-flex justify-content-between mt-3">
                        <div class="">
                            <img src="../assets/images/avada-music-logo.png" class="w-75 ">
                        </div>
                        <div class="nav-wrapper">
                            <NavBar />
                        </div>
                    </div>
                    <div class="title-section col-8 text-center">
                        <h1 class="main-title">Untold Stories</h1>
                        <p>There is an untold story behind every favourite song</p>
                        <div>
                            <button class=" left-button">
                                LATEST ALBUM
                            </button>
                            <button class="right-button">
                                LIVE DATES
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

header {
    height: 100vh;
    background-image: url("../src/assets/images/home_slider.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
}

.title-section {
    margin: 0 auto;
    margin-top: 4.5rem;

    .main-title {
        font-size: 5.5rem;
    }

    p {
        font-size: 1rem;
        color: white;
        padding-bottom: 1rem;
        font-style: italic;
    }
}

button {
    padding: 0.5rem 1.5rem;
    margin-right: 0.5rem;
    color: white;
}

.left-button {
    background-color: $divider-color;
    border: none;
    transition: 0.3s;
}

.right-button {
    border: 0.5px-solid white;
    background: none;
    transition: 0.3s;

}

.right-button:hover,
.left-button:hover {
    color: black;
    border: none;
    background-color: white;
}
</style>