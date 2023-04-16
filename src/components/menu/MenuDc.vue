<script>
    export default {
        name: 'MenuDc',
        data() {
            return {
                menu: [
                    {
                        text: 'Terms Of Use',
                        href: '#',
                    },
                    {
                        text: 'Privacy policy (New)',
                        href: '#',
                    },
                    {
                        text: 'Ad Choices',
                        href: '#',
                    },
                    {
                        text: 'Advertaising',
                        href: '#',
                    },
                    {
                        text: 'Jobs',
                        href: '#',
                    },
                    {
                        text: 'Subscriptions',
                        href: '#',
                    },
                    {
                        text: 'CPSC Certificates',
                        href: '#',
                    },
                    {
                        text: 'Ratings',
                        href: '#',
                    },
                    {
                        text: 'Shop Help',
                        href: '#',
                    },
                    {
                        text: 'Contact Us',
                        href: '#',
                    },
                ]
            }
       }
    }
</script>

<template>
    <div class="row">
        <div class="col">
            <div class="item" v-for="item in menu">
                <ul>
                    <li>
                        <a :href="item.href">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

ul {
        padding: 0;
        margin: 0.25rem;
        
        a {
            color: $gray;
        }
    }
</style>