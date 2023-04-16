<script>
import SocialMedia from '../social-media/SocialMedia.vue'
export default {
    components: {
        SocialMedia
    },
    name: 'FooterBottom',
}
</script>

<template>
    <footer>

        <div class="container">
            <div class="row">
                <div class="col">
                    <button type="button" class="btn text-uppercase fw-semibold">Sign-up now!</button>
                </div>
                <div class="col">
                    <SocialMedia/>
                </div>
            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

footer {
    background-color: $footerBottom;
    padding: 2rem 0;

    .btn {
        padding: 0.5rem 0.75rem;
        border: 3px solid $primary;
        border-radius: 0;
        color: $light;
    }
}

</style>