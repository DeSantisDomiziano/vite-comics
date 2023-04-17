<script>
    export default {
        name: 'SeriesComicbooks',
        props: {
            thumb: String,
            price: String,
            series: String,
            type: String
        }
    }
</script>


<template>
    
        <div class="col-2">
            <div class="card border-0">
                <img :src="thumb" :alt="type">
                <div class="card-body">
                <p class="card-text fw-semibold text-white">{{ series }}</p>
                </div>
            </div>
        </div>
    
    
    
</template>

<style lang="scss" scoped>

.col-2 {
/*     color: black;
 */    padding: 2.25rem 0.5rem;

    .card {
        background: transparent;
        min-height: 270px;


        p {
            text-transform: uppercase;
        }
    }
    
    
    img {
        min-height: 260px;
        aspect-ratio: 1;
        object-fit: cover;
    }
}

</style>