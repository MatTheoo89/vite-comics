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

                    <div class="col">
                        <h2>Dc commics</h2>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>Tv</li>
                            <li>Games</li>
                            <li>Collectibles</li>
                            <li>News</li>
                        </ul>

                        <h2>Shop</h2>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>

                    <div class="col">
                        <h2>Dc</h2>
                        <ul>
                            <li>Term Of USe</li>
                            <li>Privacy policy (new)</li>
                            <li>Ad Choises</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Rating</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>

                    <div class="col">
                        <h2>Sites</h2>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazione</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>

                </div>

                <div class="col-right">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
                </div>

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
    height: 80%;
    background-image: url('../src/assets/img/footer-bg.jpg');
    .container{
        height: 100%;
        display: flex;
        justify-content: space-between;
        .col-left{
            display: flex;
            width: 45%;
            height: 100%;
            .col{
                width: calc(100% / 3);
                padding: 30px 15px;
                margin: 10px;
                h2{
                    color: #fff;
                    text-transform: uppercase;
                    font-weight: 600;
                    margin-bottom: 10px;

                }
                ul{
                    list-style: none;
                    li{
                        color: grey;
                        font-size: .75rem;
                        margin-bottom: 7px;
                        &:hover{
                            color: #fff;
                            cursor: pointer;
                        }
                        &:last-child{
                            margin-bottom: 20px;
                        }
                    }
                }
            }
        }
        .col-right{
            overflow-y:hidden ;
            img{
                transform: translateY(-18%);
            }
        }
    }
}

.footer-bottom{
    height: 20%;
    background-color: #444444;
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
            border:3px solid $blue-color;
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
