<template>
    <section>
        <div class="container">

            <ol class="shop-wrap">
                <li class="shop-item" v-for="(item, i) in shopList" :key="i">
                    <figure class="shop-item-logo">
                        <img :src="require('../assets/img/' + item.image)" alt="">
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
@import '../assets/scss/mixins.scss';

section {
    width: 100%;
    background-color: $primaryColor;
    padding: 50px 10px;
    color: #fff;

    .shop-wrap {
        display: flex;
        align-items: center;
        gap: 20px 1%;
        padding: 10px 40px;

        .shop-item {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 10px;
            width: calc(96% / 5);

            .shop-item-logo {
                height: 60px;

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

@media screen and (max-width: 1200px) {

    .shop-item {
        flex-direction: column;
    }
}

@media screen and (max-width: 992px) {

    section {

        .shop-wrap{

            flex-wrap: wrap;

            .shop-item {
                width: calc(97% / 4);
            }
        }
    }
}

@media screen and (max-width: 576px) {

    section {

        .shop-wrap{

            flex-wrap: wrap;

            .shop-item {
                width: calc(99% / 2);
            }
        }
    }
}
    
</style>