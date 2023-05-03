<script>
  import headerComp from './components/headerComp.vue'
  import contentComp from './components/contentComp.vue'
  export default{
    name: 'App',
    components: {
      headerComp,
      contentComp
    }
  }
</script>

<template>
  <headerComp/>
  <contentComp/>
</template>

<style>

</style>
