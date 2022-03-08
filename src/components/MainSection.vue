<template>
    <section>
        <div class="container">
        <ol class="shop-wrap">
            <li class="shop-item" v-for="(item, i) in shopList" :key="i">
                <figure class="shop-item-logo">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                </figure>
                <div class="shop-item-title">
                    <a :href="item.ancora">
                        <h4>{{ item.title }}</h4>
                    </a>
                </div>
            </li>
        </ol>
        </div>
    </section>
</template>

<script>
export default {
    name: 'mainSection',

    data() {
        return {
            shopList: [
                {
                    image: 'buy-comics-digital-comics.png',
                    ancora: '#',
                    title: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    ancora: '#',
                    title: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    ancora: '#',
                    title: 'subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    ancora: '#',
                    title: 'comic shop locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    ancora: '#',
                    title: 'dc power visa'
                },
            ],
        }
    }
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
        gap: 1%;
        padding: 10px 40px;

        .shop-item {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            width: calc(96% / 5);

            .shop-item-logo {
                width: 70px;
                height: 70px;

                img {
                    margin: 0 auto;
                }
            }

            .shop-item-title {
                text-transform: uppercase;
                font-size: 14px;
                flex-grow: 1;
                white-space: nowrap;

                h4 {
                    font-weight: 400;
                    padding: 5px;
                }
            }
        }
    }
}
    
</style>