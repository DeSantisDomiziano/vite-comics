<script>
    export default {
        name: 'SocialMedia',
        data() {
            return{
                socials: [
                    {
                        src: 'footer-facebook',
                        href: '#'
                    },
                    {
                        src: 'footer-periscope',
                        href: '#'
                    },
                    {
                        src: 'footer-pinterest',
                        href: '#'
                    },
                    {
                        src: 'footer-twitter',
                        href: '#'
                    },
                    {
                        src: 'footer-youtube',
                        href: '#'
                    },
                ]
            }
        },
        methods: {
            getImageUrl(name) {
                return new URL(`../../assets/img/${name}.png`, import.meta.url).href
            }
        }      
    }
</script>

<template>

    
        
        <ul class="d-flex justify-content-end">
            <li>
                <h5 class="text-uppercase fw-semibold mt-2 me-4">follow us</h5>
            </li>
            <li class="p-1" v-for="social in socials">
                <img :src="getImageUrl(social.src)" :alt="social.src">
            </li>
        </ul>
    
    
    
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

h5 {
    float: left;
    color: $primary;
}
</style>