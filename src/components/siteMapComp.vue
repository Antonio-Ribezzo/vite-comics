<script>
  export default{
    name: 'siteMapComp',
    data(){
        return{
            siteItems:[
                {
                    title: 'DC COMICS',
                    items:[
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title: 'SHOP',
                    items:[
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },
                {
                    title: 'DC',
                    items:[
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title: 'SITES',
                    items:[
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]
                }
            ]
        }
    }
  }
</script>

<template>
    <section class="text-white">
        <div class="container d-flex justify-content-between align-items-center">
            <!-- lista sx -->
            <div id="listSx" class="d-flex justify-content-between align items-center">
                <div v-for="(el,index) in siteItems" :key="index">
                    <h4>{{ el.title }}</h4>
                    <ul>
                        <li v-for="(el,index) in siteItems[index].items" :key="index">
                            <a href="#">{{ el }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- logo dx -->
            <div>
                <img id="logoLarge" src="/img/dc-logo-bg.png" alt="logo-large">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // importo il foglio di stile principale
    @use "../style/main.scss" as *;

    section{
        background-image: url('/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
    }

    #listSx{
        height: 80%;
        width: 50%;
    }

    ul{
        margin: 0;
        padding: 0;
        
        li{
            list-style: none;
            font-family: 'Khula', sans-serif;
            a{
                text-decoration: none;
                color: grey;
                &:hover{
                    background-color: lightblue;
                }
            }
        }
    }
</style>
