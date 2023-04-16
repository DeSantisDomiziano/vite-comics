<script>
    export default {
       name: 'SiteHeader',
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
   
        <nav class="navbar navbar-expand-sm navbar-light justify-content-between pb-0">
            <div class="container">
                <a class="navbar-brand" href="#">
                    <img src="../assets/img/dc-logo.png" alt="">
                </a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarID"
                    aria-controls="navbarID" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse flex-grow-0 text-uppercase fw-bold" id="navbarID">
                    <div class="navbar-nav" v-for="nav in menu">
                        <a class="nav-link active" aria-current="page" :href="nav.href">{{nav.text}}</a>
                    </div>
                </div>
            </div>
        </nav>

</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as*;

a {
    img {
        max-height: 60px;
    }

    &:hover {
        border-bottom: 3px solid $primary;
    }
}

#navbarID {
    height: 70px;
    padding-top: 0.8rem;

    .navbar-nav {
        height: 100%;
    }
}

</style>