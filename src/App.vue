<script>
  import headerComp from './components/headerComp.vue'
  import contentComp from './components/contentComp.vue'
  import storeComp from './components/storeComp.vue'
  export default{
    name: 'App',
    components: {
      headerComp,
      contentComp,
      storeComp
    }
  }
</script>

<template>
  <headerComp/>
  <contentComp/>
  <storeComp/>
</template>

<style>

</style>
