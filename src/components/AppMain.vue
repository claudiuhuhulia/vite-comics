<script>
export default {
    props: {
        series: Array
    },

}
</script>


<template>
    <section class="series">
        <div class="series-title">
            CURRENT SERIES
        </div>
        <div class="container">
            <div class="card-container">
                <div v-for="serie in series" :key="serie.series" class="card">
                    <figure>
                        <img :src="serie.thumb" alt="serie">
                    </figure>
                    <h3> {{ serie.series }}</h3>
                </div>

            </div>

        </div>
        <div class="load-btn">LOAD MORE</div>
    </section>
</template>

<style lang="scss" scoped>
.series {
    background-color: black;
    height: 650px;
    display: flex;
    align-items: center;
    flex-direction: column;
    position: relative;
}

.series-title {
    position: absolute;
    top: -25px;
    left: 330px;
    color: white;
    background-color: #0c7cec;
    padding: 10px 20px;
    font-weight: bold;
    font-size: 1.5rem;
    cursor: pointer;
}

.load-btn {
    background-color: #0c7cec;
    color: white;
    padding: 10px 60px;
    cursor: pointer;
    font-weight: bold;
}

.card-container {
    display: flex;
    flex-wrap: wrap;
    padding-top: 50px;
    padding-bottom: 50px;

    .card {
        flex-basis: calc(100% / 6);
        cursor: pointer;
    }

    figure {
        height: 175px;
        overflow: hidden;

        img {
            height: 141%;
            object-fit: cover;
            object-position: 50% 0%;
        }
    }
}

h3 {
    color: white;
    margin-top: 10px;
    font-weight: 400;
    font-size: 1rem;
    width: 170px;
}
</style>