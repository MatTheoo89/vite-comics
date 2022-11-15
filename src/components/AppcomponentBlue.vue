<script>
export default {
    name: 'AppcomponentBlue'
}
</script>

<template>
    <div class="main-bottom">

        <div class="container">

            <div class="card">

                <img src="../assets/img/buy-comics-digital-comics.png" alt="buy-comics-digital-comics.png">

                <h3>digital comics</h3>

            </div>

            <div class="card">

                <img src="../assets/img/buy-comics-merchandise.png" alt="buy-comics-merchandise.png">

                <h3>dc merchandise</h3>

            </div>

            <div class="card">

                <img src="../assets/img/buy-comics-subscriptions.png" alt="buy-comics-subscriptions.png">

                <h3>subscription</h3>

            </div>

            <div class="card">

                <img src="../assets/img/buy-comics-shop-locator.png" alt="buy-comics-shop-locator.png">

                <h3>comics shop locator</h3>

            </div>

            <div class="card">

                <img src="../assets/img/buy-dc-power-visa.svg" alt="buy-dc-power-visa.svg">

                <h3>dc power visa</h3>

            </div>
            
            
            
            
            

        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;

    .main-bottom{
        height: 150px;
        background-color: $blue-color;
        .container{
            display: flex;
            justify-content: space-around;
            align-items: center;
            height: 100%;
            .card{
                display: flex;
                align-items: center;
                padding: 20px;
                img{
                    width: 50px;
                    margin-right: 20px;
                }
                h3{
                    color: #fff;
                    text-transform: uppercase;
                    font-weight: 400;
                    font-size: .9rem;
                }
            }
        }
    }
    
</style>