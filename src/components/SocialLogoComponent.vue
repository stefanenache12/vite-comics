<script>
export default {
    name: "SocialLogoComponent",
    data() {
        return {
            socialLogos: [
                'src/vue-dc-comics/img/footer-facebook.png',
                'src/vue-dc-comics/img/footer-periscope.png',
                'src/vue-dc-comics/img/footer-pinterest.png',
                'src/vue-dc-comics/img/footer-twitter.png',
                'src/vue-dc-comics/img/footer-youtube.png'
            ]

        }
    },
    methods: {

    }
}
</script>

<template>
    <div class="social-logos">
        <div v-for="singleSocialLogo in socialLogos" class="logos">
            <img :src="singleSocialLogo" alt="">
        </div>

    </div>
</template>

<style lang="scss" scoped>
    .logos {
        padding: .3125rem;
    }

</style>