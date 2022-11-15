<script>
export default {
    name: "AppFooter",
};
</script>

<template>

    <footer>

        <div class="footer-top">
            <div class="container">

                <div class="col-left">

                </div>

                <!-- <div class="col-right">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
                </div> -->

            </div>
        </div>

        <div class="footer-bottom">
            <div class="container">
                <button>Sign-up now!</button>
                <div class="social">
                    <h3>Follow us</h3>
                    <div class="icons-socials">
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>

@use '../style/partials/variables' as *;

footer{
    height: 480px;
}

.footer-top{
    display: flex;
    justify-content: space-between;
    height: 80%;
    background-image: url('../src/assets/img/footer-bg.jpg');
}

.footer-bottom{
    height: 20%;
    background-color: rgb(80, 79, 79);
    .container{
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        button{
            text-transform: uppercase;
            color: #fff;
            font-size: .8rem;
            font-weight: 600;
            border:2px solid $blue-color;
            background-color: transparent;
            padding: 7px 10px;
        }
        .social{
            display: flex;
            align-items: center;
            h3{
            color: $blue-color;
            text-transform: uppercase;
            margin-right: 15px;
        }
        img{
            width: 1.7rem;
            filter: brightness(1.6);
            margin-right: 10px;
        }
        }
        
    }
}



</style>
