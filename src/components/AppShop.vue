<script>
export default {
    data() {
        return {
        }
    },
    props: {
        ShopImages: Array
    },
    methods: {
        getImagePath(image) {
            const url = new URL(image, import.meta.url)
            return url.href
        }
    }

}
</script>

<template>
    <!-- shop section -->
    <section class="bgcshop">
        <div class="container">
            <ul>
                <li v-for="image in ShopImages" :key="image">
                    <img :src="getImagePath(image.image)" alt="s">
                    <h3>{{ image.text }}</h3>
                </li>
            </ul>
        </div>
    </section>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/mixin' as *;

ul {
    @include center-flex;
    cursor: pointer;

    li {
        @include center-flex;
        padding-left: 35px;
        padding-right: 35px;
    }
}

h3 {
    font-weight: 400;
    font-size: 0.8rem;
    color: white;
    padding-left: 15px;
}

img {
    height: 70px;
}

.bgcshop {
    @include center-flex;
    background-color: #0c7cec;
    height: 180px;
}
</style>