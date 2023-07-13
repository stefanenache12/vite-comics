<script>
export default {
    name: "HeaderComponent",
    data() {{
        return {
            menu: [
                'CHARCTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBILIES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ],

            logo: [
                'src/vue-dc-comics/img/dc-logo.png'
            ]
        }

        }
    },
    methods: {

    }
}
</script>

<template>
    <header>

        <div>
            <img :src="logo" alt="Logo DC Comics">
        </div>

        <div  class="menu">
            <div v-for="singleMenu in menu" class="single-menu">
                {{ singleMenu }}
            </div>
        </div>
        
    </header>
</template>

<style lang="scss" scoped>
    @use "src/assets/scss/header.scss";
</style>