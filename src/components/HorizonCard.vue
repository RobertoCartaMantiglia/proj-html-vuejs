<script>
export default {
    name: 'HorizonCard',
    data() {
        return {
            horizontalCardsList: [
                {
                    thumb: 'blog_music_techo-600x300.jpg',
                    title: 'Tecnology and Music',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur non debitis beatae totam facilis a at animi, libero fuga possimus culpa enim provident impedit.'
                },
                {
                    thumb: 'blog_flavor_rock-600x300.jpg',
                    title: 'The flavour of Rock',
                    text: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Veniam sed ipsa consequuntur non debitis beatae totam facilis a at animi, libero fuga possimus culpa enim provident impedit.'
                },
            ]
        }
    },
    methods: {
        getImagePath(imagePath) {
            return new URL(`../assets/images${imagePath}`, import.meta.url).href;
        }
    },
}
</script>
<template>
    <div>

    </div>
</template>
<style lang="scss" scoped>

</style>