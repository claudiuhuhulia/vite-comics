<script>
export default {
    data() {
        return {
            navLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]

        }
    }
} 
</script>

<template>
    <!-- header -->
    <header class="container">
        <figure>
            <img src="../assets/img/dc-logo.png" alt="logo">
        </figure>
        <nav>
            <ul>
                <li v-for="link in navLinks" :key="link.text"><a :href=link.url>{{ link.text }}</a></li>
            </ul>
        </nav>
    </header>


    <!-- content section -->
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixin' as *;


header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 140px;
}

ul {
    @include center-flex;

    li {
        font-weight: bold;



        a {
            color: black;
            padding: 55px 10px;
            text-transform: uppercase;

            &:hover {
                border-bottom: 4px solid #0c7cec;
                color: #0c7cec;
            }
        }
    }
}
</style>