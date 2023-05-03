<script>
  import headerComp from './components/headerComp.vue'
  import contentComp from './components/contentComp.vue'
  import storeComp from './components/storeComp.vue'
  import siyeMapComp from './components/siteMapComp.vue'
  export default{
    name: 'App',
    components: {
      headerComp,
      contentComp,
      storeComp,
      siyeMapComp
    }
  }
</script>

<template>
  <headerComp/>
  <contentComp/>
  <storeComp/>
  <siyeMapComp/>
</template>

<style>

</style>
