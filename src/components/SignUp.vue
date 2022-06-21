<template>
    <div>
        <div class="sign-up">
            <div class="container d-flex justify-content-between align-items-center">
                <button class="btn btn-outline-primary rounded-0 text-uppercase text-white">Sign-up now!</button>

                <div class="links text-primary text-uppercase fw-bold">
                    <span class="pe-2">Follow Us</span>
                    <a href="javascript.void(0)">
                        <img v-for="(img, i) in socialArray" :key="i" :src="`img/${img.image}.png`" :alt="`Icona social di ${img.name}`" class="ps-3">
                    </a>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SignUp',
    data() {
        return {
            socialArray: [
        {
            name: 'Facebook',
            image: 'footer-facebook',
        },
        {
            name: 'Twitter',
            image: 'footer-twitter',
        },
        {
            name: 'Youtube',
            image: 'footer-youtube',
        },
        {
            name: 'Pinterest',
            image: 'footer-pinterest',
        },
        {
            name: 'Periscope',
            image: 'footer-periscope',
        },
    ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .sign-up {
        background-color: #303030;
        padding: 1rem;
    }
</style>