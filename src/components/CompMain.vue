<script>
export default {
    name: 'CompMain'
}
</script>
<template>
    <main>
        <section class="first-section">
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
                    <div class="col-6 m-auto pt-3">
                        <h2 class="paragraph-title pb-4">Latest Band News</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                            laudantium,
                            dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                            ullam.

                        </p>
                    </div>
                </div>
            </div>
            <div class="container">
                <div class="row ">
                    <div class="col-9 d-flex m-auto justify-content-center">
                        <div class="col-6 d-flex flex-wrap left-side">
                            <div class="card horizontal-card">

                            </div>

                            <div class="card vertical-card">

                            </div>

                            <div class="card vertical-card">

                            </div>
                            <div class="card horizontal-card">

                            </div>

                        </div>
                        <div class="col-4 right-side">
                            <div class="col-3 card vertical-card">

                            </div>
                            <div class="col-3 card vertical-card">

                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

.first-section {
    height: 225px;
    background-color: $bg-color-small-section;
}

.paragraph-title {
    border-bottom: 1px solid $words;
}

.main-section {
    background-color: $bg-principal-section;
}

.horizontal-card {
    width: 100%;
    height: 180px;
    background-color: $bg-color-small-section;
}

.vertical-card {
    height: 300px;
    width: 50%;
    background-color: $bg-color-small-section;
}

.right-side {
    .vertical-card {
        width: 100%;
        height: 50%;
    }
}
</style>