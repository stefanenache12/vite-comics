<script>
export default {
    name: "MainCardsComponent",
    data() {
        return {

        }
    },
    methods: {

    },
    props: {
        singleseriesImage: String,
        singleseriesTitle: String
    }
}
</script>

<template>

    <div class="single-card">
        <div>
            <img
                :src="singleseriesImage"
                :alt="singleseriesTitle"
            />
        </div>
        <h4>{{ singleseriesTitle }}</h4>
    </div>
  
</template>

<style lang="scss" scoped>

    img {
        width: 100%;
        height: 200px;
        object-fit: cover;
        padding: 5px;
    }
 
</style>