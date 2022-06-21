<template>
    <div class="banner">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-2" v-for="(img, i) in bannerArray" :key="i">
                    <a href="javascript:void(O)">
                        <img :src="`img/${img.immagine}.${img.estensione}`" :alt="`immagine di ${img.nome}`" :class="{'smaller' : i === 4}">
                        <span class="text-uppercase">{{ img.nome }}</span>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TheBanner',
    data() {
        return {
            bannerArray: [
                {
                    nome: 'Digital Comics',
                    immagine: 'buy-comics-digital-comics',
                    estensione: 'png',
                },
                {
                    nome: 'Dc Merchandise',
                    immagine: 'buy-comics-merchandise',
                    estensione: 'png',
                },
                {
                    nome: 'Subscription',
                    immagine: 'buy-comics-subscriptions',
                    estensione: 'png',
                },
                {
                    nome: 'Comic Shop Locator',
                    immagine: 'buy-comics-shop-locator',
                    estensione: 'png',
                },
                {
                    nome: 'Dc Power Visa',
                    immagine: 'buy-dc-power-visa',
                    estensione: 'svg',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .banner {
        background-color: #0282F9;
        padding: 2.5rem;
        font-family: Arial, Helvetica, sans-serif;

        a {
            text-decoration: none;
            color: white;
        }

        img {
            height: 40px;
            margin-right: 10px;
        }

        .smaller {
            width: 40px;
        }

        span {
            font-size: .7rem;
        }

    }
</style>