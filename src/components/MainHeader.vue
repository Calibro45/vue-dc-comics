<template>
    <header class="main-header">
        <div class="container">

            <figure class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>

            <nav class="main-nav">
            <ol>
                <li :class="['nav-link',(activeIndex === i) ? 'active' : '' ]" 
                v-for="(link, i) in navLink" :key="i"
                @click="activeElement(i)">
                    <a :href="link.anchor">{{ link.textLink }}</a>
                </li>
            </ol>
            </nav>
            
        </div>
    </header>
</template>

<script>
export default {
    name: 'mainHeader',

    data() {
        return {
            activeIndex: 0,
            navLink: [
                {
                    anchor: '#',
                    textLink: 'character'
                },
                 {
                    anchor: '#',
                    textLink: 'comics'
                },
                 {
                    anchor: '#',
                    textLink: 'movies'
                },
                 {
                    anchor: '#',
                    textLink: 'tv'
                },
                 {
                    anchor: '#',
                    textLink: 'games'
                },
                 {
                    anchor: '#',
                    textLink: 'collectibles'
                },
                 {
                    anchor: '#',
                    textLink: 'videos'
                },
                 {
                    anchor: '#',
                    textLink: 'fans'
                },
                 {
                    anchor: '#',
                    textLink: 'news'
                },
                 {
                    anchor: '#',
                    textLink: 'shop'
                },

            ],
        };
    },

    methods: {
        activeElement: function(i) {
            this.activeIndex = i;
        },
    }
}
</script>

<style lang="scss" scoped>

.main-header {
    padding: 0 10px;

    .container {
        display: flex;
        justify-content: space-between;
        min-height: 110px;
        gap: 20px;

        .logo {
            width: 85px;
            height: 85px;
            align-self: center;
            flex-shrink: 0;
        }

        .main-nav {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;

            ol {
                display: contents;
            }

            .nav-link {
                text-transform: uppercase;
                font-size: 14px;
                font-weight: 700;
                color: #464646;
                position: relative;

                a {
                    display: block;
                    height: 100%;
                    display: flex;
                    align-items: center;
                }

                &.active, &:hover {
                    color: #0282f9;

                    a::after {
                        content: '';
                        display: block;
                        height: 5px;
                        background-color: #0282f9;
                        position: absolute;
                        bottom: 0;
                        left: 0;
                        right: 0;
                    }
                }
            }
        }
    }
}


</style>