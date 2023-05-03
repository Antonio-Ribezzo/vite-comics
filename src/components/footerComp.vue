<script>
  export default{
    name: 'footerComp'
  }
</script>

<template>
    <footer>
        <div class="container py-4 d-flex justify-content-between align-items-center">
            <!-- footer sx -->
            <div>
                <button class="text-uppercase text-white px-3 py-2">sign-up now!</button>
            </div>
            <!-- footer dx -->
            <div class="d-flex justify-content-between align-items-center">
                <span class="text-uppercase colorLightBlue mx-3">follow us</span>
                <img src="/img/footer-facebook.png" alt="facebook-logo" class="mx-2">
                <img src="/img/footer-twitter.png" alt="twitter-logo" class="mx-2">
                <img src="/img/footer-youtube.png" alt="youtube-logo" class="mx-2">
                <img src="/img/footer-pinterest.png" alt="pinterest-logo" class="mx-2">
                <img src="/img/footer-periscope.png" alt="periscope-logo" class="mx-2">
            </div>


        </div>
    </footer>
</template>

<style lang="scss" scoped>
    // importo il foglio di stile principale
    @use "../style/main.scss" as *;

    footer{
        background-color: #303030;
    }

    button{
        background-color: #303030;
        border: 0.1rem solid $colorLightBlue;
    }

    span{
        font-family: 'Asap Condensed', sans-serif;
        font-weight: 600;
        font-size: 1.5rem;
    }

</style>
