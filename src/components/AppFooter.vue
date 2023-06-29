<script>
export default {
    data() {
        return {
            comicsItems: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop',
            ],
            dcItems: [
                'Term Of Use',
                'Privacy policy(New)',
                'Ad Choises',
                'Advertising',
                'Jobs',
                'Talent Workshop',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us',
            ],
            sitesItems: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa',
            ],
            shopItems: [
                'Shop DC',
                'Shop DC Collectibles'

            ]

        }
    }
}
</script>

<template>
    <footer class="bgc-footer">
        <!-- footer nav -->
        <section class="container footer-flex ">
            <nav>
                <div class="comicsnav">
                    <h1>DC COMICS</h1>
                    <ul>
                        <li v-for="item in comicsItems">{{ item }}</li>
                    </ul>
                    <h1>SHOP</h1>
                    <ul>
                        <li v-for="item in shopItems">{{ item }}</li>
                    </ul>
                </div>

                <div class="dcnav">
                    <h1>DC</h1>
                    <ul>
                        <li v-for="item in dcItems">{{ item }}</li>
                    </ul>
                </div>
                <div class="shopnav">
                    <h1>SITES</h1>
                    <ul>
                        <li v-for="item in sitesItems">{{ item }}</li>
                    </ul>
                </div>
            </nav>

            <div class="bgc-right"></div>
        </section>

    </footer>
</template>

<style scoped>
.bgc-footer {
    height: 380px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

.bgc-right {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    width: 47%;
    background-position: center;
}

.footer-flex {
    display: flex;
    justify-content: space-between;
    height: 100%;

}

nav {
    display: flex;
    margin-top: 30px;
}



ul li {
    color: grey;
    font-size: 0.8rem;
}

h1 {
    color: white;
    margin-top: 10px;
    margin-bottom: 10px;

}

.comicsnav,
.dcnav,
.sitesnav {
    margin-right: 15px;
    margin-left: 15px;
}
</style>