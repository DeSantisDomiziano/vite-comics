<script>
    export default {
        name: 'MenuSites',
        data() {
            return {
                menu: [
                    {
                        text: 'DC',
                        href: '#',
                    },
                    {
                        text: 'MAD Magazine',
                        href: '#',
                    },
                    {
                        text: 'DC Kids',
                        href: '#',
                    },
                    {
                        text: 'DC Universe',
                        href: '#',
                    },
                    {
                        text: 'DC Power Visa',
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