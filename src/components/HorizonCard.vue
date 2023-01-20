<script>
export default {
    name: 'HorizonCard',
    data() {
        return {
            horizontalCardsList: [
                {
                    thumb: 'blog_music_techo-800x400.jpg',
                    title: 'Tecnology and Music',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur non debitis beatae totam facilis a at animi.'
                },
                {
                    thumb: 'blog_flavor_rock-600x300.jpg',
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
        <img :src="getImagePath(card.thumb)" class="" alt="#">
        <div class="card-info">
            <h3>{{ card.title }}</h3>
            <p>{{ card.text }}</p>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.horizon-card {
    width: 100%;
    height: 100%;

    img {
        width: 100%;
        height: 60%;
    }



}
</style>