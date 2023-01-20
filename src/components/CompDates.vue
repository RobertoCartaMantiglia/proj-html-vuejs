<script>
export default {
    name: 'CompDates',
    data() {
        return {
            datesList: [
                {
                    text: '17/08/2020 GEM FESTIVAL 2020 ANAKALIA, GEORGIA'
                },
                {
                    text: '24/09/2020 GROOVEFEST DOMINICAL REPUBLIC'
                },
                {
                    text: '31/10/2020 OASIS FESTVAL 2020 MARRAKECH, MOROCCO'
                },
                {
                    text: '07/11/2020 MOGA FESTIVAL - ESSAOURIA, MOROCCO'
                },
                {
                    text: '10/12/2020 ENVISION FESTIVAL - UVITA, COSTA RICA'
                },

            ]
        }
    }
}
</script>
<template>
    <div class="container">
        <div class="row">
            <div class="col-6 m-auto pt-3">
                <h2>Live Dates</h2>
                <div class="paragraph-underline m-auto my-4"></div>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum quia voluptates
                    laudantium,
                    dignissimos unde nobis adipisci illum pariatur provident neque nam, iure accusamus
                    ullam.
                </p>
            </div>
        </div>
        <div class="col-10 m-auto">
            <div class="date-list">
                <ul class="mt-4">
                    <li v-for="dateElement in datesList">
                        <span class="text-white px-2">+</span>
                        {{ dateElement.text }}
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

.paragraph-underline {
    width: 180px;
    border: 1px solid $background-social;
}

.date-list {
    color: $li-date-color;
    text-align: left;

    ul {
        list-style-type: none;

        li {
            background-color: $bg-color-small-section;
            padding: 0.5rem;
            font-size: 0.8rem;
            margin-bottom: 0.6rem;
        }
    }
}
</style>