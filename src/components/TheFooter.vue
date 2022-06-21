<template>
    <div>
        <footer>
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="py-4 align-items-center">
                            <h6 class="text-uppercase fw-bold">Dc Comics</h6>
                            <ul class="list-unstyled">
                                <li v-for="linkDc in dcComicsLinks" :key="linkDc">{{ linkDc.name }}</li>
                            </ul>
                            <h6 class="text-uppercase fw-bold">Shop</h6>
                            <ul class="list-unstyled">
                                <li v-for="linkShop in shopLinks" :key="linkShop">{{ linkShop.name }}</li>
                            </ul>
                        </div>
                    </div>

                    <div class="col">
                        <img src="/img/dc-logo-bg.png" alt="">
                    </div>

                </div>
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'TheFooter',
    data() {
        return {
            dcComicsLinks: [
                {
                    name: 'Characters',
                    href: '#',
                },
                {
                    name: 'Comics',
                    href: '#',
                },
                {
                    name: 'Movies',
                    href: '#',
                },
                {
                    name: 'Tv',
                    href: '#',
                },
                {
                    name: 'Games',
                    href: '#',
                },
                {
                    name: 'Videos',
                    href: '#',
                },
                {
                    name: 'News',
                    href: '#',
                },
            ],
            shopLinks: [
                {
                    name: 'Shop DC',
                    href: '#',
                },
                {
                    name: 'Shop DC Collectibles',
                    href: '#',
                }
            ],
            dcLinks: [
                {
                    name: 'Terms Of Use',
                    href: '#',
                },
                {
                    name: 'Privacy Policy (New)',
                    href: '#',
                },
                {
                    name: 'Ad Choices',
                    href: '#',
                },
                {
                    name: 'Advertising',
                    href: '#',
                },
                {
                    name: 'Jobs',
                    href: '#',
                },
                {
                    name: 'Subscriptions',
                    href: '#',
                },
                {
                    name: 'Talent Workshops',
                    href: '#',
                },
                {
                    name: 'CPSC Certificates',
                    href: '#',
                },
                {
                    name: 'Ratings',
                    href: '#',
                },
                {
                    name: 'Shop Help',
                    href: '#',
                },
                {
                    name: 'Contact Us',
                    href: '#',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    footer {
        background-image: url('/public/img/footer-bg.jpg');
        background-size: cover;
        color: white;
        overflow: hidden;
        position: relative;

        ul li {
            font-family: Arial, Helvetica, sans-serif;
            font-size: .6rem;
            color: #797979;
        }

        img {
            height: 400px;
            position: absolute;
            top: -70px;
        }
    }
</style>