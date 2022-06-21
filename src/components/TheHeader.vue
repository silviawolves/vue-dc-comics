<template>
    <div>
        <header>
            <div class="container">
                <div class="my-navbar">
                    <img src="/img/dc-logo.png" alt="">
                    <ul class="list-unstyled m-0 d-flex">
                        <li class="text-uppercase fw-bold mx-3" v-for="(link, i) in linkNav" :key="i">
                            <a href="javascript:void(0)">{{ link.name }}
                                <div class="active"></div>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </header>
    </div>
</template>

<script>
export default {
    name: 'TheHeader',
    data() {
        return {
            linkNav: [
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
                    name: 'Collectibles',
                    href: '#',
                },
                {
                    name: 'Videos',
                    href: '#',
                },
                {
                    name: 'Fans',
                    href: '#',
                },
                {
                    name: 'News',
                    href: '#',
                },
                {
                    name: 'Shop',
                    href: '#',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    header {

        .my-navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            
            img {
                height: 60px;
            }

            ul li {
                font-size: .8rem;
                padding: 2rem 0;
                text-align: center;
                position: relative;

                a {
                    height: 100%;
                    text-decoration: none;
                    opacity: 60%;
                    color: black;

                    &:focus {
                        color: #0282F9;
                        opacity: 100%;
                    }

                    &:focus .active {
                        display: block;
                    }
                    
                    .active {
                        width: 100%;
                        display: none;
                        border-bottom: 4px solid #0282F9;
                        position: absolute;
                        bottom: 0;
                        left: 0;
                    }
                }
            }
        } 
    }
</style>