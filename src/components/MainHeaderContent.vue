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
    <div class="background">
        <div class="container">
            <a href="#">
                <h2>{{ message }} </h2>
            </a>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.background {
    background-color: #1C1C1C;
}

div {
    height: 150px;
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