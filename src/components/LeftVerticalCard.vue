<script>
export default {
    name: 'LeftVerticalCard',
    data() {
        return {
            verticalLeftCardsList: [
                {
                    thumb: 'blog-post3-600x900.jpg',
                    title: 'Taking it back to the old school',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur.'
                },
                {
                    thumb: 'blog-post4-600x900.jpg',
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
    <div class="vertical-card" v-for="card in verticalLeftCardsList">
        <img :src="getImagePath(card.thumb)" alt="#">
        <div class="card-info p-3">
            <h4 class="pt-3">{{ card.title }}</h4>
            <p>{{ card.text }} </p>
        </div>
    </div>

</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;


// .vertical-card-wrap {
//     height: 450px;
//     display: flex;
//     width: calc((100% / 2) - 0.5rem);
//     margin-right: 0.5rem;
//     background-color: $bg-color-small-section;

// }

img {
    width: 100%;
}

h4 {
    color: $card-title;
    font-size: 0.9rem;
    font-weight: bold;
}
</style>