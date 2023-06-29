<script>
export default {
    data() {
        return {
            ShopSections: [
                {
                    img: '<img src="../assets/img/buy-comics-digital-comics.png" alt="">',
                    text: 'DIGITAL COMICS'
                }
            ]
        }
    },
    methods: {
        getImagePath() {
            const url = new URL(`../assets/img/${this.img}`, import.meta.url)
            console.log(url)
        }
    }
}
</script>

<template>
    <!-- shop section -->
    <section class="bgcshop">
        <div class="container">
            <ul>
                <li v-for="section in ShopSections" :key="section.text">{{ section.text }}</li>
            </ul>
        </div>
    </section>
</template>

<style scoped>
.bgcshop {
    background-color: #0c7cec;
    height: 180px;
}
</style>