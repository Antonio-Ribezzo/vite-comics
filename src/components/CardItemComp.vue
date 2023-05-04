<script>
    export default{
        name: 'CardItemComp',
        props: ['ArrayCard']
    }
</script>

<template>
    <li class="my-4">
        <a class="text-white" href="#">
            <img :src="ArrayCard.thumb" :alt="ArrayCard.series">
            <p class="mt-2 text-start">{{ ArrayCard.series }}</p>
            <span class="m-0 text-start">{{ ArrayCard.price }}</span>
            <span class="m-0 text-start">{{ ArrayCard.type }}</span>
        </a>
    </li>
</template>

<style lang="scss" scoped>
    li{
        list-style: none;
        width: calc((100% / 6) - 1rem);
        a{
            text-decoration: none;
            &:hover{
                filter: brightness(1.2);
            }

            img{
                height: 10rem;
                width: 100%;
            }

            span{
                display: block;
                font-size: 0.7rem;
                color: grey;
                text-transform: capitalize;
            }
        }
    }
</style>