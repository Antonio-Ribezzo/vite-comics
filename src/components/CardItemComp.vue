<script>
    export default{
        name: 'CardItemComp',
        props: ['ArrayCard']
    }
</script>

<template>
    <li class="my-4">
        <img :src="ArrayCard.thumb" alt="">
        <p class="mt-3 text-start">{{ ArrayCard.series }}</p>
    </li>
</template>

<style lang="scss" scoped>
    li{
        list-style: none;
        width: calc((100% / 6) - 1rem);
        img{
            height: 10rem;
            width: 100%;
        }
    }
</style>