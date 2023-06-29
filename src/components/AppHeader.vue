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

    <section class="container content"></section>
</template>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
}

ul {
    display: flex;
    justify-content: center;
    align-items: center;

}

ul li {
    list-style-type: none;
    font-weight: bold;
}

ul li a {
    color: black;
    padding: 30px 10px;
}

ul li a:hover {
    border-bottom: 4px solid #0c7cec;
    color: #0c7cec;
}
</style>