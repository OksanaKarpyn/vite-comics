<script>
export default {
    name: 'DcCosmics',
    props: ['prompsCosmic'],
    data() {
        return {
        }

    },

}
</script>
<template>
    <div class="card py-2">
        <img :src="prompsCosmic.thumb" alt="foto">
        <h3 class="pt-2">{{ prompsCosmic.series }}</h3>
        <span>{{ prompsCosmic.price }}</span>
    </div>
</template>
<style lang="scss" scoped>
.card {
    width: calc(100% / 7);
    background-color: #1C1C1C;

    img {
        width: 100%;
        aspect-ratio: 1;
    }

    h3 {
        font-size: 1rem;
        color: #fff;
    }

    span {
        color: #fff;
    }
}
</style>