<template>
    <div>
        <div class="my-card">
            <div class="card-img">
                <img :src="imgUrl" :alt="`Immagine di ${imgText}`">
            </div>
            
            <div class="card-title">{{ imgText }}</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ContainerFumetti',
    props: {
        imgUrl: String,
        imgText: String,
    }
}
</script>

<style lang="scss" scoped>

.my-card {

    .card-img {
        overflow: hidden;
        aspect-ratio: 1/1;
    }

    .card-title {
        text-transform: uppercase;
        font-family: Arial, Helvetica, sans-serif;
        font-weight: normal;
        font-size: .7rem;
        padding: 1rem 0;
    }
}
</style>