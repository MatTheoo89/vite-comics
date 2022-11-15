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

            <img :src="`/dc-logo.png`" alt="dc-logo">

        </div>

        <nav>
            <ul>
                <li
                    v-for="(link, index) in navMenu"
                    :key="index">
                    <a
                        :class="{'active': link.active}"
                        :href="link.href">{{link.text}}
                    </a>
                </li>
            </ul>
        </nav>

    </div>

</header>

</template>

<style lang="scss" scoped>

@use '../style/partials/variables' as *;

header{
    background-color: #fff;
    
    .container{
        padding: 20px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;

        nav{
            ul{
                display: flex;
                list-style: none;
                li{
                    position: relative;
                    font-weight: 600;
                    padding: 0 10px;
                    text-transform: uppercase;
                    height: 100%;
                    
                    }
                    a{
                        display: inline-block;
                        color: $grey-main;
                        text-decoration: none;
                        &:hover,
                        &.active{
                            color: $blue-color;
                        }
                        &.active::after{
                            content: '';
                            position: absolute;
                            left: 50%;
                            bottom: -350%;
                            width: 100%;
                            height: 5px;
                            transform: translate(-50%, -50%);
                            background-color:$blue-color;
                    }
                }
            }
        }
    }
}
</style>