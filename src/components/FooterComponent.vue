<script>
import SocialLogoComponent from './SocialLogoComponent.vue';
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
            dcComics: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ],
            dc: [
                'Terms Of Use',
                'Privacy Policy(New)',
                'Ad Choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],
            shop: [
                'Shop Dc',
                'Shop Dc Collectibles'
            ],
            sites: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC universe',
                'DC Power Visa'
            ]


        }
    },
    methods: {
    },
    components:{
        SocialLogoComponent,
    }
}
</script>

<template>
    <footer>
        <div class="section-1">
            <div class="container" >
                <div v-for="singleImg in buyComicsImg" class="img-container">
                    <img :src="singleImg.img" alt="">
                    <h6>{{ singleImg.name }}</h6>
                </div>
            </div>
        </div>

        <div class="section-2">
            <div class="footer-container">
                <div class="footer-lists">

                    <div class="footer-list">
                        <div>
                            <h4>DC COMICS</h4>
                            <ul>
                                <li v-for="singleLinkDcComics in dcComics">
                                    <a href="#">
                                        {{ singleLinkDcComics }}
                                    </a>
                                </li>
                            </ul>
                        </div>

                        <div>
                            <h4>SHOP</h4>
                            <ul>
                                <li v-for="singleShoplink in shop">
                                    <a href="#">
                                        {{ singleShoplink }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="footer-list">
                        <div>
                            <h4>DC</h4>
                            <ul>
                                <li v-for="singleDcLink in dc">
                                    <a href="#">
                                        {{ singleDcLink }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="footer-list">
                        <div>
                            <h4>SITES</h4>
                            <ul>
                                <li v-for="singleSite in sites">
                                    <a href="#">
                                        {{ singleSite }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="footer-logo">
                        <img src="src/vue-dc-comics/img/dc-logo-bg.png" alt="">
                    </div>

                </div>
            </div>
        </div>

        <div class="section-3">

            <div class="container-section-3">
                <div>
                <button>SING-UP NOW!</button>
                </div>

                <div class="social-logos">
                    <h3>FOLLOW US</h3>
                    <SocialLogoComponent/>
                </div>

            </div>

            

        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @use "src/assets/scss/partials/footer.scss";

    button {
        padding: 10px 20px;
        background-color: #303030;
        border: 2px solid #0282F9;
        color: white;
        font-weight: bold;
    }
</style>