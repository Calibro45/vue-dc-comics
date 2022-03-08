<template>
    <footer>
        <section id="contatti">
            <div class="container">
                <div class="contact-wrap">
                    <h3 class="contact-title">{{ linkTitle[0] }}</h3>
                    <ol class="contact-list">
                        <li class="contact-link" v-for="(links, i) in footerLink" :key="i">
                            <a :href="links.ancora">{{ links.link }}</a>
                        </li>
                    </ol>
                    <h3 class="contact-title">{{ linkTitle[1] }}</h3>
                    <ol class="contact-list">
                        <li class="contact-link" v-for="(links, i) in shopLink" :key="i">
                            <a :href="links.ancora">{{ links.link }}</a>
                        </li>
                    </ol>
                </div>
                <div class="contact-wrap">
                    <h3 class="contact-title">{{ linkTitle[2] }}</h3>
                    <ol class="contact-list">
                        <li class="contact-link" v-for="(links, i) in dcLink" :key="i">
                            <a :href="links.ancora">{{ links.link }}</a>
                        </li>
                    </ol>
                </div>
                <div class="contact-wrap">
                    <h3 class="contact-title">{{ linkTitle[3] }}</h3>
                    <ol class="contact-list">
                        <li class="contact-link" v-for="(links, i) in siteLinks" :key="i">
                            <a :href="links.ancora">{{ links.link }}</a>
                        </li>
                    </ol>
                </div>
            </div>
        </section>
        <section id="info">
            <div class="container">
                <div>
                    <button class="sign-in">sign-up now!</button>
                </div>
                <ol class="social">
                    <li class="social-item">
                        <h3>Follow Us</h3>
                    </li>
                    <li class="social-item" v-for="(icon, i) in socialLink" :key="i">
                        <a href="#">
                            <img :src="require('../assets/img/' + icon.image)" alt="">
                        </a>
                    </li>
                </ol>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'mainFooter',

    data() {
        return {
            linkTitle: ['dc comics', 'shop', 'dc', 'sites'],
            footerLink: [
                {
                    link: 'character',
                    ancora: '#',
                },
                {
                    link: 'comics',
                    ancora: '#',
                },
                {
                    link: 'movies',
                    ancora: '#',
                },
                {
                    link: 'tv',
                    ancora: '#',
                },
                {
                    link: 'games',
                    ancora: '#',
                },
                {
                    link: 'videos',
                    ancora: '#',
                },
                {
                    link: 'news',
                    ancora: '#',
                },
            ],

            shopLink: [
                {
                    link: 'shop DC',
                    ancora: '#',
                },
                {
                    link: 'shop DC collectibles',
                    ancora: '#',
                },
            ],

            dcLink: [
                {
                    link: 'Term Of Use',
                    ancora: '#',
                },
                {
                    link: 'Privacy policy (New)',
                    ancora: '#',
                },
                {
                    link: 'Ad Choises',
                    ancora: '#',
                },
                {
                    link: 'Adversiting',
                    ancora: '#',
                },
                {
                    link: 'Jobs',
                    ancora: '#',
                },
                {
                    link: 'Subscriptions',
                    ancora: '#',
                },
                {
                    link: 'Talent Workshops',
                    ancora: '#',
                },
                {
                    link: 'CPSC Certificates',
                    ancora: '#',
                },
                {
                    link: 'Ratings',
                    ancora: '#',
                },
                {
                    link: 'Shop Help',
                    ancora: '#',
                },
                {
                    link: 'Contact Us',
                    ancora: '#',
                },
            ],

            siteLinks: [
                {
                    link: 'DC',
                    ancora: '#',
                },
                {
                    link: 'MAD Magazine',
                    ancora: '#',
                },
                {
                    link: 'DC Kids',
                    ancora: '#',
                },
                {
                    link: 'DC Universe',
                    ancora: '#',
                },
                {
                    link: 'DC Power Visa',
                    ancora: '#',
                }
            ],

            socialLink: [
                {
                    image: 'footer-facebook.png',
                    ancora: '#'
                },
                {
                    image: 'footer-twitter.png',
                    ancora: '#'
                },
                {
                    image: 'footer-youtube.png',
                    ancora: '#'
                },
                {
                    image: 'footer-pinterest.png',
                    ancora: '#'
                },
                {
                    image: 'footer-periscope.png',
                    ancora: '#'
                },
            ]
        };
    },
}
</script>

<style lang="scss" scped>

#contatti {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-position: top;

    .container {
        display: flex;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
        gap: 10px;
    }

    .contact-wrap {
        width: 12%;
        padding: 50px 10px;

        .contact-title {
            text-transform: uppercase;
            color: #fff;
            margin-bottom: 20px;
        }

        .contact-list {
            color: #959595;
            font-size: 14px;
            margin-bottom: 20px;

            .contact-link {
                padding: 5px 0px;
            }
        }
    }
}

#info {
    background-color: #303030;
    padding: 25px 5px;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;

        .sign-in {
            background-color: transparent;
            color: #fff;
            padding: 15px;
            border: 2px solid #027adc;
            text-transform: uppercase;
            font-weight: 700;

            &:hover {
                cursor: pointer;
            }
        }

        .social {
            display: flex;
            align-items: center;
            gap: 20px;

            .social-item {
                padding: 5px 8px;

                h3 {
                    color: #027adc;
                    text-transform: uppercase;
                }
            }
        }
    }
}
    
</style>