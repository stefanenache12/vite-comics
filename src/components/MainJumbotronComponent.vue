<script>
export default {
    name: "MainJumbotronComponent",
    data() {
        return {
            Jumbotron: {
                img: 'src/vue-dc-comics/img/jumbotron.jpg',
            }
        }
    },
    methods: {

    }
}
</script>

<template>
    <div class="jumbotron">
        <img :src="Jumbotron.img" alt="Jumbotron">
        <button>CURENT SERIES</button>
    </div>
    
</template>

<style lang="scss" scoped>

.jumbotron {
    position: relative;

    button {
        position: absolute;
        padding: 10px;
        background-color: #0282F9;
        border-radius: 0;
        border: none;
        color: white;
        bottom: -10px;
        left: 245px;
        }

    img {
        width: 100%;
        height: 300px;
        object-fit: cover;
        object-position: top;
    }

}



</style>