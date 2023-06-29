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
                <img src="../assets/img/footer-facebook.png" alt="fb">
            </div>
        </div>
    </footer>
</template>

<style scoped>
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

.signup-btn h3 {
    color: white;
}

.followus h3 {
    color: #0c7cec;
}

.followus {
    display: flex;
    align-items: center;
}

.signup-btn {
    border: 2px solid #0c7cec;
    padding: 15px;
}
</style>