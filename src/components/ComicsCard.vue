<template>
    <div class="comics-card-wrap">
        <figure class="card-header">
            <img :src="thumbs" alt="">
        </figure>
        <div class="card-body">
            <h4>{{ series }}</h4>
        </div>
    </div>
</template>

<script>
export default {
    name: 'comicsCard',
    props: ['thumbs', 'series'],
}
</script>


<style lang="scss" scoped>

.comics-card-wrap {
    width: calc(95% / 6);
    padding: 5px;

    .card-header {
        
        img {
            aspect-ratio: 1;
            object-fit: cover;
            object-position: center;
            
        }
    }

    .card-body {
        color: #fff;
        text-transform: uppercase;
        padding: 25px 0px;

        h4 {
            font-weight: 400;
            font-size: 14px;
        }
    }
}

@media screen and (max-width: 768px) {
    
    .comics-card-wrap {
        width: calc(98% / 3);
    }
}

@media screen and (max-width: 576px) {
    
    .comics-card-wrap {
        width: 100%;
    }
}

</style>