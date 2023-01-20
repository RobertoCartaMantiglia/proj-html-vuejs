<script>
export default {
    name: 'DividerLink',
    data() {
        return {
            linksList: [
                {
                    text: 'VIEW ALL LATEST NEWS',
                },
            ],
        }
    },
}
</script>
<template>
    <div class="divider">
        <div class="container-fluid">
            <div class="row align-items-center">
                <div class="col-4 m-auto">
                    <div v-for="link in linksList">
                        <a href="#">
                            {{ link.text }}
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

.divider {
    background-color: $divider-color;
    transition: background-color 0.5s;

    a {
        color: white;
        font-size: 0.9rem;
    }
}

.divider:hover {
    background-color: white;

    a {
        color: black;
    }
}
</style>