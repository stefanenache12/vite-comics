<script>
import MainJumbotronComponent from './MainJumbotronComponent.vue';
import MainCardsComponent from './MainCardsComponent.vue';

export default {
    name: "MainComponent",
    data() {
        return {

        }
    },
    methods: {

    },
    components: {
        MainJumbotronComponent,
        MainCardsComponent,
    }
}
</script>

<template>
    <main>
        <MainJumbotronComponent/>
        <MainCardsComponent/>
    </main>
</template>

<style lang="scss" scoped>

main {
    background-color: #1C1C1C;
    text-align: center;
    color: white;
    
}

</style>