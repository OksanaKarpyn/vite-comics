<script>
export default {
    name: 'MainHeaderContent',
    data() {
        return {
            message: '-->Content goes here<--'
        }
    }
}
</script>
<template>
    <div class="container">
        <a href="#">
            <h2>{{ message }} </h2>
        </a>
    </div>
</template>
<style lang="scss" scoped>
div {
    height: 150px;
    background-color: rgb(24, 23, 23);
    display: flex;
    align-items: center;

    a {
        text-decoration: none;
        display: inline-block;

        h2 {
            color: #fff;
        }
    }
}
</style>