<script>
export default {
    props: {
        series: Array
    },

}
</script>


<template>
    <section class="series">
        <div class="container">
            <div class="card-container">
                <div class="card">
                    <img src="https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Action_Comics_Vol_1_1000.jpg/revision/latest?cb=20180412200923"
                        alt="">
                    <h3> Action Comics</h3>
                </div>
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
.series {
    background-color: black;
}

.card-container {
    display: flex;
    flex-wrap: wrap;

    .card {
        flex-basis: calc(100% / 6);
        height: 200px;

        img {
            height: 100%;
            object-fit: none;
            object-position: 50% 0%;
        }
    }
}
</style>