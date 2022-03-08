<template>
    <footer>
        <section id="contatti">
            <div class="container">
                <div class="contact-wrap">
                    <h3 class="contact-title">dc comics</h3>
                    <ol class="contact-list">
                        <li class="contact-link">
                            <a href="#">link</a>
                        </li>
                    </ol>
                    <h3 class="contact-title">shop</h3>
                    <ol class="contact-list">
                        <li class="contact-link">
                            <a href="#">link</a>
                        </li>
                    </ol>
                </div>
                <div class="contact-wrap">
                    <h3 class="contact-title">dc</h3>
                    <ol class="contact-list">
                        <li class="contact-link">
                            <a href="#">link</a>
                        </li>
                    </ol>
                </div>
                <div class="contact-wrap">
                    <h3 class="contact-title">sites</h3>
                    <ol class="contact-list">
                        <li class="contact-link">
                            <a href="#">link</a>
                        </li>
                    </ol>
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'mainFooter',
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
        gap: 20px;

    }

    .contact-wrap {
        width: 10%;
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
                padding: 5px 0;
            }
        }
    }
}
    
</style>