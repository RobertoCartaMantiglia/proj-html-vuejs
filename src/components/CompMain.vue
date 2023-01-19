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
                    <div class="col-8 m-auto pt-3">
                        <h2 class="paragraph-title pb-4">Music is LIfe</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                            laudantium,
                            dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                            ullam.
                            Veniam
                            sed quod aliquid sunt consequuntur.
                        </p>
                    </div>
                </div>
            </div>
        </section>
        <section class="main-section">
            <div class="container">
                <div class="row">
                    <div class="col-8 m-auto pt-3">
                        <h2 class="paragraph-title pb-4">Latest Band News</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                            laudantium,
                            dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                            ullam.
                            Veniam sed quod aliquid sunt consequuntur.
                        </p>
                    </div>
                    <div class="col-8">

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
    height: 700px;
    background-color: $bg-principal-section;
}
</style>