<script>
import BannerMain from './main-components/BannerMain.vue'
export default {
    components: {
        BannerMain
    },
    name: 'SiteMain',        
}
</script>

<template>

    <section id="top">
        <div class="container">

        </div>
    </section>
    <!-- #/SECTION TOP -->

    <BannerMain/>
    <!-- #/SECTION BOTTOM -->
    
</template>


<style lang="scss" scoped>
section {
    background-color: black;
    color: white;
}


</style>