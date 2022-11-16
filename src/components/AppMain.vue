<script>
export default {
    name: "AppMain",
};
</script>

<template>

    <main>

        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        </div>

        <div class="container">

            <button class="top">Current Series</button>
            
            <div class="card-area">

                <button>Load More</button>
            </div>
            
        </div>

    </main>

</template>

<style lang="scss" scoped>

    @use '../style/partials/variables' as *;

    .jumbotron{
        background-color: red;
        height: 500px;
        object-fit: cover;
        object-position: center;
        overflow: hidden;
        img{
            width: 100%;
        }
    }

    button{
        border: none;
        outline: none;
        background-color: $blue-color;
        padding: 10px 25px;
        color: #fff;
        font-size: 1.2rem;
        text-transform: uppercase;
        text-align: center;
        &.top{
            font-weight: 500;
            transform: translateY(-230%);
        }
    }

    .card-area{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .container{
        color: #fff;
        padding: 80px 0;
    }

</style>
