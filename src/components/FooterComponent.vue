<script>
export default {
    name: "FooterComponent",
    data() {
        return {
            buyComicsImg: [
                {
                    img:'src/vue-dc-comics/img/buy-comics-digital-comics.png',
                    name:'DIGITAL COMICS'
                },
                {
                    img:'src/vue-dc-comics/img/buy-comics-merchandise.png',
                    name:'DC MERCHANDISE'
                },
                {
                    img:'src/vue-dc-comics/img/buy-comics-shop-locator.png',
                    name:'SUBSCRIPTION'
                },
                {
                    img:'src/vue-dc-comics/img/buy-comics-subscriptions.png',
                    name:'COMIC SHOP LOCATOR'
                },
                {
                    img:'src/vue-dc-comics/img/buy-dc-power-visa.svg',
                    name:'DC POWER VISA'
                }
                
            ],


        }
    },
    methods: {
    }
}
</script>

<template>
    <div class="shop">
        <div class="container" >
            <div v-for="singleImg in buyComicsImg" class="img-container">
                <img :src="singleImg.img" alt="">
                <h6>{{ singleImg.name }}</h6>
            </div>
        </div>
    </div>

    <footer>
        FOOTER
    </footer>
</template>

<style lang="scss" scoped>
    @use "src/assets/scss/partials/footer.scss";
</style>