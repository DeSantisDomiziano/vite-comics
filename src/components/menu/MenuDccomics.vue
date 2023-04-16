<script>
    export default {
        name: 'MenuDccomics',
        data() {
            return {
                menu: [
                    {
                        text: 'Characters',
                        href: '#',
                    },
                    {
                        text: 'Comics',
                        href: '#',
                    },
                    {
                        text: 'Movies',
                        href: '#',
                    },
                    {
                        text: 'TV',
                        href: '#',
                    },
                    {
                        text: 'Games',
                        href: '#',
                    },
                    {
                        text: 'Collectibles',
                        href: '#',
                    },
                    {
                        text: 'Videos',
                        href: '#',
                    },
                    {
                        text: 'Fans',
                        href: '#',
                    },
                    {
                        text: 'News',
                        href: '#',
                    },
                    {
                        text: 'Shop',
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