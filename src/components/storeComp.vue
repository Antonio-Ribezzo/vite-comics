<script>
  export default{
    name: 'storeComp',
    data(){
        return{
            storeItems:[
                {
                    icon: '/img/buy-comics-digital-comics.png',
                    nome:'DIGITAL COMICS',
                    url: '/digital-comics'
                },
                {
                    icon: '/img/buy-comics-merchandise.png',
                    nome:'DC MERCHANDISE',
                    url: '/dc-merchandise'
                },
                {
                    icon: '/img/buy-comics-subscriptions.png',
                    nome:'SUBSCRIPTION',
                    url: '/subscription'
                },
                {
                    icon: '/img/buy-comics-shop-locator.png',
                    nome:'COMIC SHOP LOCATOR',
                    url: '/comic-shop-locator'
                },
                {
                    icon: '/img/buy-dc-power-visa.svg',
                    nome:'DC POWER VISA',
                    url: '/dc-power-visa'
                }
            ]
        }
    }
  }
</script>

<template>
    <section>
        <div class="container py-5">
            <ul class="d-flex justify-content-around align-items-center">
                <li v-for="(el,index) in storeItems" :key="index">
                    <a :href="el.url" class="d-flex justify-content-center align-items-center">
                        <img :src="el.icon" :alt="el.name + 'icon'">
                        <span class="ms-3">{{ el.nome }}</span>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // importo il foglio di stile principale
    @use "../style/main.scss" as *;

    section{
        background-color: $colorLightBlue;
    }

    ul{
        margin: 0;
        li{
            list-style: none;
            font-family: 'Khula', sans-serif;
            a{
                text-decoration: none;
                color: white;
                &:hover{
                    background-color: lightblue;
                }
                img{
                    max-height: 3rem;
                    max-width:3rem;
                }
            }
        }
    }
</style>
