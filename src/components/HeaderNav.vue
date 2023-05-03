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
<style  lang="scss" scoped>
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    min-height: 150px;

    ul {

        display: flex;
        list-style-type: none;

        li {
            margin-top: 20px;
            margin: 0px 20px;
            max-height: 100px;
            display: inline-block;
            align-items: center;

            a {
                font-size: 1rem;
                font-weight: bold;
                color: black;
                text-decoration: none;
                height: 50px;

                &:hover {
                    border-bottom: 5px solid blue;
                    padding-bottom: 70px;
                    color: blue;
                }
            }

        }
    }
}
</style>