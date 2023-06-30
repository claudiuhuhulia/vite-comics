<script>
export default {

}
</script>

<template>
    <footer>
        <div class="footer-flex container">
            <div class="signup-btn">
                <h3>SIGN UP NOW!</h3>
            </div>
            <div class="followus">
                <h3> FOLLOW US </h3>
                <img src="../assets/img/footer-facebook.png" alt="fb">
                <img src="../assets/img/footer-periscope.png" alt="pr">
                <img src="../assets/img/footer-pinterest.png" alt="pi">
                <img src="../assets/img/footer-twitter.png" alt="tw">
                <img src="../assets/img/footer-youtube.png" alt="yt">

            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    height: 140px;
    background-color: #303030;
}

.footer-flex {
    display: flex;
    justify-content: space-between;
    height: 100%;
    align-items: center;
}

.followus h3 {
    color: #0c7cec;
    margin-right: 15px;
}

.followus {
    display: flex;
    align-items: center;

    img {
        margin-left: 10px;
    }
}

.signup-btn {
    border: 2px solid #0c7cec;
    padding: 15px;

    h3 {
        color: white;
    }
}
</style>