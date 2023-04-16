<script>
import BannerMain from './main-components/BannerMain.vue'
import CurrentSeries from './main-components/CurrentSeries.vue'
export default {
    components: {
        BannerMain,
        CurrentSeries
    },
    name: 'SiteMain',        
}
</script>

<template>

    <CurrentSeries/>
    <!-- #/SECTION TOP -->

    <BannerMain/>
    <!-- #/SECTION BOTTOM -->
    
</template>