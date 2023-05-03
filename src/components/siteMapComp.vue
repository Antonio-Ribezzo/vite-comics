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
        <div id="container0" class="container d-flex justify-content-between align-items-center">
            <!-- lista sx -->
            <div class="d-flex justify-content-between align items-center">
                <div>
                    <h4>{{ siteItems[0].title }}</h4>
                    <ul>
                        <li v-for="(el, index) in siteItems[0].items" :key="index">
                            <a href="#">{{ el }}</a>
                        </li>
                    </ul>

                    <h4 class="mt-2">{{ siteItems[1].title }}</h4>
                    <ul>
                        <li v-for="(el, index) in siteItems[1].items" :key="index">
                            <a href="#">{{ el }}</a>
                        </li>
                    </ul>
                </div>
                <div class="ms-4">
                    <h4>{{ siteItems[2].title }}</h4>
                    <ul>
                        <li v-for="(el, index) in siteItems[2].items" :key="index">
                            <a href="#">{{ el }}</a>
                        </li>
                    </ul>
                </div>
                <div class="ms-4">
                    <h4>{{ siteItems[3].title }}</h4>
                    <ul>
                        <li v-for="(el, index) in siteItems[3].items" :key="index">
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
        height: 25rem;
        width: 100%;
        #container0{
            height: 100%;
            width: 100%;
        }
    }

    h4{
        font-family: 'Asap Condensed', sans-serif;
        font-weight: 600;
    }

    ul{
        margin: 0;
        padding: 0;
        
        li{
            list-style: none;
            font-family: 'Khula', sans-serif;
            font-size: 0.8rem;
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
