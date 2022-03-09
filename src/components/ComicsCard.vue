<template>
    <div class="comics-card-wrap">
        <figure class="card-header">
            <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
        </figure>
        <div class="card-body">
            <h4>action comics</h4>
        </div>
    </div>
</template>

<script>
export default {
    name: 'comicsCard',

}
</script>

<style lang="scss" scoped>

.comics-card-wrap {
    width: calc(95% / 6);
    padding: 5px;

    .card-header {
        aspect-ratio: 1;
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

</style>