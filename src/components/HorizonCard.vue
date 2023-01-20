<script>
export default {
    name: 'HorizonCard',
    data() {
        return {
            horizontalCardsList: [
                {
                    thumb: 'blog_music_techo-800x400.jpg',
                    title: 'Technology and Music',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur non debitis beatae totam facilis a at animi.'
                },
                {
                    thumb: 'blog_flavor_rock-800x400.jpg',
                    title: 'The flavour of Rock',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur non debitis beatae totam facilis a at animi.'
                },
            ]
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
    <div class="horizon-card" v-for="card in horizontalCardsList">
        <img :src="getImagePath(card.thumb)" alt="#">
        <div class="card-info p-2">
            <h4 class="pt-3">{{ card.title }}</h4>
            <p>{{ card.text }}</p>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

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
    }
}
</style>