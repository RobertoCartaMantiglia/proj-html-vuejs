<script>
export default {
    name: 'VerticalCardRight',
    data() {
        return {
            verticalRightCardsList: [
                {
                    thumb: 'blog-post1-600x900.jpg',
                    title: 'Taking it back to the old school',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur.'
                },
                {
                    thumb: 'blog-post2-200x300.jpg',
                    title: 'Sharing the stage with the legends',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur.'
                },
            ],
        }
    },
    methods: {
        getImagePath(imagePath) {
            return new URL(`../assets/images/${imagePath}`, import.meta.url).href;
        }
    },
}
</script>
<template>
    <div class="vertical-card-wrap" v-for="card in verticalRightCardsList">
        <div class="vertical-card pb-2">
            <img :src="getImagePath(card.thumb)" alt="#">
            <div class="card-info p-3">
                <h4 class="pt-3">{{ card.title }}</h4>
                <p>{{ card.text }} </p>
            </div>
        </div>
    </div>

</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;


.vertical-card-wrap {
    width: 100%;
    height: calc((100% / 2) - 1rem);
    margin-bottom: 0.5rem;
    background-color: $bg-color-small-section;
    text-align: left;

    img {
        width: 100%;

    }
}

h4 {
    color: $card-title;
    font-size: 0.9rem;
    font-weight: bold;
}
</style>
