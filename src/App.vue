<script>
  import headerComp from './components/headerComp.vue'
  import contentComp from './components/contentComp.vue'
  import storeComp from './components/storeComp.vue'
  import siteMapComp from './components/siteMapComp.vue'
  import footerComp from './components/footerComp.vue'
  export default{
    name: 'App',
    components: {
      headerComp,
      contentComp,
      storeComp,
      siteMapComp,
      footerComp
    }
  }
</script>

<template>
  <headerComp/>
  <contentComp/>
  <storeComp/>
  <siteMapComp/>
  <footerComp/>
</template>

<style>

</style>
