<script>
export default {
    name: 'AppCard',
    props: {
        cardItem : String
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


<style lang="scss">
    @use '../style/partials/variables' as *;

</style>