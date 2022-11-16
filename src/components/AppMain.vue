<script>
import AppCard from './AppCard.vue';
import articles from '../data/dc-comics'
export default {
    name: "AppMain",
    components: { AppCard },
    data(){
        return{
            articles
        }
    }
}
</script>

<template>

    <main>

        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotron">
        </div>

        <div class="container">

            <button class="top">Current Series</button>
            
            <div class="card-area">

                <AppCard v-for="(article, index) in articles" :key="index" :cardItem="article"/>

            </div>
            
            
        </div>
        
        <div class="button">
            <button>Load More</button>
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
        &.top{
            font-weight: 500;
            transform: translateY(-170%);
        }
    }

    .card-area{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin-bottom: 20px;
    }

    .container{
        color: #fff;
        padding: 50px 0;
    }
    
    .button{
    text-align: center;
    margin-bottom: 50px;
    }
</style>
