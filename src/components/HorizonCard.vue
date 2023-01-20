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

</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;
</style>