<script>
    export default {
        name: 'BannerMain',
        data() {
            return {
                banner: [
                    {
                        src: 'buy-comics-digital-comics.png',
                        text: 'Digital Comics',
                    },
                    {
                        src: 'buy-comics-merchandise.png',
                        text: 'DC Merchandise',
                    },
                    {
                        src: 'buy-comics-shop-locator.png',
                        text: 'Subscription',
                    },
                    {
                        src: 'buy-comics-subscriptions.png',
                        text: 'Comic Shop Locator',
                    },
                    {
                        src: 'buy-dc-power-visa.svg',
                        text: 'DC Power Visa',
                    },
                ]
            }
        },
        methods: {
            getImageUrl(name) {
                return new URL(`../../assets/img/${name}`, import.meta.url).href
            }
        }      
   }
</script>


<template>

<section>
        <div class="container">
            <div class="row py-3">
                <div class="col" v-for="item in banner">
                    <img :src="getImageUrl(item.src)" :alt="item.text">
                    <p class="text-uppercase d-flex ps-2 align-items-center h-100  m-0">{{ item.text }}</p>
                </div>
            </div>
        </div>
    </section>
    
</template>


<style lang="scss" scoped>
    img {
        max-height: 50px;
        float: left;
    }

    p {
        font-size: 0.8rem;
    }
    .col:nth-child(5) {
        img {
            max-width: 70px;
            position: relative;
            top: 0.25rem
        }
    }

</style>