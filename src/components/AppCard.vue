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
        width: calc(100% / 6);
        padding: 20px 10px;
        .card-image{
            overflow: hidden;
            margin-bottom: 10px;
            text-align: center;
            img{
                width: 200px;
                height: 200px;
                object-fit: cover;
                object-position: top;
        }
    }
    span{
        text-align: left;
        text-transform: uppercase;
        font-size: .8rem;
        padding-left: 4px;
    }
    }

</style>