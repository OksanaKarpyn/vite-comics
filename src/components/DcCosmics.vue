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
    <div class="card">
        <img :src="prompsCosmic.thumb" alt="foto">
        <h3>{{ prompsCosmic.series }}</h3>
        <span>{{ prompsCosmic.price }}</span>
    </div>
</template>
<style lang="scss" scoped>
.card {
    width: calc(100% / 7);



    h3 {
        font-size: 1rem;
    }
}
</style>