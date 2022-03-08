<template>
    <header>
        <div class="container nav-wrapper">
            <figure class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <ol class="main-nav">
                <li :class="['nav-link',(activeIndex === i) ? 'active' : '' ]" 
                v-for="(link, i) in navLink" :key="i"
                @click="activeElement(i)">
                    <a :href="link.anchor">{{ link.textLink }}</a>
                </li>
            </ol>
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

.nav-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 15px 5px;

    .logo {
        width: 85px;
        height: 85px;
        flex-shrink: 0;
    }

    .main-nav {
        display: flex;
        align-items: center;
        gap: 30px;
        flex-wrap: wrap;

        .nav-link {
            padding: 5px 10px;
            text-transform: uppercase;
            font-size: 14px;
            font-weight: 700;
            position: relative;
            color: #464646;

            &.active {
                color: #579cfa
            }

            &.active::after {
                content: '';
                display: block;
                height: 5px;
                background-color: #579cfa;
                width: calc(100% - 20px);
                position: absolute;
                bottom: -100%;
            }

            &:hover {
                cursor: pointer;
                color: #579cfa;
            }
        }
    }
}


</style>