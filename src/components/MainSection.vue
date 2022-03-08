<template>
    <section>
        <div class="container">
        <ol class="shop-wrap">
            <li class="shop-item">
                <figure class="shop-item-logo">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                </figure>
                <div class="shop-item-title">
                    <h4>digital comics</h4>
                </div>
            </li>
            <li class="shop-item">
                <figure class="shop-item-logo">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                </figure>
                <div class="shop-item-title">
                    <h4>digital comics</h4>
                </div>
            </li>
            <li class="shop-item">
                <figure class="shop-item-logo">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                </figure>
                <div class="shop-item-title">
                    <h4>digital comics</h4>
                </div>
            </li>
            <li class="shop-item">
                <figure class="shop-item-logo">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                </figure>
                <div class="shop-item-title">
                    <h4>digital comics</h4>
                </div>
            </li>
            <li class="shop-item">
                <figure class="shop-item-logo">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                </figure>
                <div class="shop-item-title">
                    <h4>digital comics</h4>
                </div>
            </li>
        </ol>
        </div>
    </section>
</template>

<script>
export default {
    name: 'mainSection',
    
}
</script>

<style lang="scss" scoped>

section {
    width: 100%;
    background-color: #0282f9;
    padding: 50px 10px;
    color: #fff;

    .shop-wrap {
        display: flex;
        align-items: center;
        gap: 2%;
        padding: 10px 40px;

        .shop-item {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            width: calc(92% / 5);
            gap: 20px;

            .shop-item-logo {
                width: 70px;
                height: 70px;
            }

            .shop-item-title {
                text-transform: uppercase;
                font-size: 14px;

                h4 {
                    font-weight: 400;
                }
            }
        }
    }
}
    
</style>