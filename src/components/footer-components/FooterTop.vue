<script>
import MenuDccomics from '../menu/MenuDccomics.vue'
import MenuShop from '../menu/MenuShop.vue'
import MenuDc from '../menu/MenuDc.vue'
import MenuSites from '../menu/MenuSites.vue'
export default {
    components: {
        MenuDccomics,
        MenuShop,
        MenuDc,
        MenuSites
    },
    name: 'FooterTop',
}
</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-6 py-5">
                
                    <div class="row row-cols-3">

                        <div class="col">
                            <h3>DC COMICS</h3>
                            <MenuDccomics/>
                            <h3 class="mt-4">SHOP</h3>
                            <MenuShop/>
                        </div>

                        <div class="col">
                            <h3>DC</h3>
                            <MenuDc/>
                            
                        </div>

                        <div class="col">
                            <h3>SITES</h3>
                            <MenuSites/>
                            
                        </div>

                        
                    </div>
                </div>
                <div class="col-6" id="logo"></div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

section{
   background-image: url('../../assets/img/footer-bg.jpg');
   background-repeat: no-repeat;
   background-size: cover;

    h3 {
        color: $light;
        margin: 0.5rem 0 0 0;
    }

    #logo {
        background-image: url('../../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: left;
    }
}

</style>