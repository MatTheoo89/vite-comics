<script>
export default {
    name: 'AppCard',
    props: {
        cardItem : Object
    }
}
</script>

<template>

<div class="card">

        <div class="card-image">

            <img :src="cardItem.thumb" :alt="cardItem.series">

        </div>

        <div class="card-text">

            <span>{{cardItem.series}}</span>

        </div>

    </div>

</template>


<style lang="scss" scoped>
    @use '../style/partials/variables' as *;

    .card{
        flex-basis: 20%;
        padding: 15px;
        .card-image{
            width: 200px;
            height: 200px;
            overflow: hidden;
            margin-bottom: 10px;
            img{
                max-width: 100%;
                object-fit: cover;
                object-position: top;
                text-align: center;
        }
    }
    span{
        text-align: left;
        text-transform: uppercase;
        font-size: .8rem;
    }
    }

</style>