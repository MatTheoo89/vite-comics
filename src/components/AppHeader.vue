<script>
export default {
    name: "AppHeader",
    data(){
        return{
            navMenu:[
                {
                    text: 'Characters',
                    href: '#',
                    active: false
                },
                {
                    text: 'Comics',
                    href: '#',
                    active: true
                },
                {
                    text: 'Movies',
                    href: '#',
                    active: false
                },
                {
                    text: 'Tv',
                    href: '#',
                    active: false
                },
                {
                    text: 'Games',
                    href: '#',
                    active: false
                },
                {
                    text: 'ollectibles',
                    href: '#',
                    active: false
                },
                {
                    text: 'Videos',
                    href: '#',
                    active: false
                },
                {
                    text: 'Fans',
                    href: '#',
                    active: false
                },
                {
                    text: 'News',
                    href: '#',
                    active: false
                },
                {
                    text: 'Shop',
                    href: '#',
                    active: false
                },
            ]
        }
    }
};
</script>

<template>

<header>
    
    <div class="container">

        <div class="logo">

            <img :src="`/dc-logo.png`" alt="">

        </div>

        <nav>
            <ul>
                <li
                    v-for="(link, index) in navMenu"
                    :key="index">
                <a href="#">${link.text}</a></li>
            </ul>
        </nav>

    </div>

</header>

</template>

<style lang="scss" scoped>
    header{
        background-color: #fff;
        padding: 20px 0;
    }
</style>
