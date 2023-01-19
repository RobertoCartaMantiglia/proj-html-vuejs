<script>
export default {
    name: 'CompFooter',
    data() {
        return {
            linksList: [
                {
                    text: 'Home'
                },
                {
                    text: 'Meet the band'
                },
                {
                    text: 'Live Dates'
                },
                {
                    text: 'Latest News'
                },
                {
                    text: 'Album'
                },
                {
                    text: 'Fans'
                },

            ],
            ItemsFooterList: [
                {
                    text: 'Copyright 2012 - 2020'
                },
                {
                    text: 'AVADA THEME BY THEMEFUSION'
                },
                {
                    text: 'ALL RIGHT RESERVED'
                },
                {
                    text: 'POWERED BY WORDPRESS'
                },

            ]

        }
    }
}
</script>
<template >
    <footer>
        <section class="footer-section first-section">
            <div class="container-fluid">
                <div class="row">
                    <div class="col-12 d-flex justify-content-between">
                        <div>
                            <img src="../assets/images/logo_footer.png" class="w-75 pt-2" alt="#">
                        </div>
                        <div>
                            <ul>
                                <li v-for="link in linksList">
                                    <a href="#">{{ link.text }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="footer-section second-section">
            <div class="container-fluid">
                <div class="row">
                    <div class="col-12 d-flex justify-content-between">
                        <div>
                            <ul>
                                <li v-for="item in ItemsFooterList">
                                    <a href="#">{{ item.text }} |</a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li>
                                    <img src="../assets/images/footer-facebook.png" alt="#">
                                </li>
                                <li>
                                    <img src="../assets/images/footer-twitter.png" alt="#">
                                </li>
                                <li>
                                    <img src="../assets/images/footer-youtube.png" alt="#">
                                </li>
                                <li>
                                    <img src="../assets/images/footer-periscope.png" alt="#">
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;

.footer-section {
    display: flex;
    align-items: center;
}

.first-section {
    height: 150px;
    background-color: $bg-color-small-section;

}

.second-section {
    height: 100px;
    background-color: $bg-principal-section;
}

ul {
    display: flex;
    list-style-type: none;
    margin-bottom: 0;

    a {
        color: $words;
        font-size: 0.7rem;
        margin-right: 0.4rem;
    }
}

li {
    margin-right: 0.4rem;

    img {
        width: 65%;
    }
}
</style>