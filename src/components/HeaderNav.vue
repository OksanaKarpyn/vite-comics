<script>
export default {
    name: 'HeaderNav',
    data() {
        return {
            listHeader: [
                {
                    name: 'CHARACTERS',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'COMICS',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'MOVIES',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'TV',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'GAMES',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'COLLECTIBLES',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'VIDEOS',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'FANS',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'NEWS',
                    url: '#',
                    visible: false,
                },
                {
                    name: 'SHOP',
                    url: '#',
                    visible: false,
                }
            ]

        }
    }
}
</script>

<template>
    <header>
        <nav class="container">
            <div class="logo">
                <img src="../../public/img/dc-logo.png" alt="foto">
            </div>
            <div>
                <ul class="">
                    <li v-for="(elem, index) in listHeader">
                        <a href="#">{{ elem.name }}</a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>
<style  lang="scss" scoped></style>