<script>
    export default{
        name: 'headerComp',
        data(){
            return{
                pages: [
                    {
                        nome: 'CHARACTERS',
                        url: '/characters',
                        current: false
                    },
                    {
                        nome: 'COMICS',
                        url: '/comics',
                        current: true
                    },
                    {
                        nome: 'MOVIES',
                        url: '/movies',
                        current: false
                    },
                    {
                        nome: 'TV',
                        url: '/tv',
                        current: false
                    },
                    {
                        nome: 'GAMES',
                        url: '/games',
                        current: false
                    },
                    {
                        nome: 'COLLECTIBLES',
                        url: '/collectibles',
                        current: false
                    },
                    {
                        nome: 'VIDEOS',
                        url: '/videos',
                        current: false
                    },
                    {
                        nome: 'FANS',
                        url: '/fans',
                        current: false
                    },
                    {
                        nome: 'NEWS',
                        url: '/news',
                        current: false
                    },
                    {
                        nome: 'SHOP',
                        url: '/shop',
                        current: false
                    }
                ]
            }
        }
    }
</script>

<template>
    <header class="container d-flex justify-content-between align-items-center">
        <!-- logo sx -->
        <div>
            <img src="/img/dc-logo.png" alt="logo-small">
        </div>
        <!-- navbar dx -->
        <nav>
            <ul class="d-flex">
                <li v-for="(el,index) in pages" :key="index" :class="(el.current) ? 'borderLightBlue' : ''" @click="(el.current == true)? false : true">
                    <a :href="el.url" :class="(el.current) ? 'colorLightBlue' : ''">{{ el.nome }}</a> 
                </li>
            </ul>
        </nav>
    </header>
    <div id="jumbotron">
    </div>
</template>

<style lang="scss" scoped>
    // importo il foglio di stile principale
    @use "../style/main.scss" as *;

    ul{
        margin: 0;
        li{
            list-style: none;
            margin: 0 1rem;
            padding: 3rem 0;
            font-family: 'Asap Condensed', sans-serif;
            font-weight: 600;
            a{
                text-decoration: none;
                color: #464646;
                &:hover{
                    background-color: #0282f99e;
                }
            }
        }
    }

    #jumbotron{
        height: 25rem;
        width: 100%;
        background-image: url('/img/jumbotron.jpg');
        background-position: top;
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>