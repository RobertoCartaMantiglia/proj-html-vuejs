
<script>

export default {

}
</script>
<template>
    <header class="jumbo">
        <section>
            <div class="row">
                <div class="col-12 d-flex justify-content-between mt-2">
                    <div class="">
                        <img src="../assets/images/avada-music-logo.png" class="w-75 ">
                    </div>
                    <div>
                        <nav class="navbar">
                            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                                data-bs-target="#navbarToggleExternalContent"
                                aria-controls="navbarToggleExternalContent" aria-expanded="false"
                                aria-label="Toggle navigation">
                                <span class="navbar-toggler-icon"></span>
                            </button>
                        </nav>
                    </div>
                </div>
                <div class="title-section col-8 text-center">
                    <h1 class="main-title">Untold Stories</h1>
                </div>
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
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
        font-size: 6rem;

    }
}
</style>