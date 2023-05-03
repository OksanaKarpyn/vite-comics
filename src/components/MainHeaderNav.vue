<script>
export default {
    name: 'MainHeaderNav',
    data() {
        return {
            itemList: [
                {
                    icon: '../../public/img/buy-comics-digital-comics.png',
                    name: 'DIGITAL COMICS',
                    visible: false,
                },
                {
                    icon: '../../public/img/buy-comics-merchandise.png',
                    name: 'DC MERCHANDISE',
                    visible: false,
                },
                {
                    icon: '../../public/img/buy-comics-subscriptions.png',
                    name: 'SABSCRIPTION',
                    visible: false,
                },
                {
                    icon: '../../public/img/buy-comics-shop-locator.png',
                    name: 'COMIC SHOP LOCATOR',
                    visible: false,
                },
                {
                    icon: '../../public/img/buy-dc-power-visa.svg',
                    name: 'DC POWER VISA',
                    visible: false,
                },
            ]

        }
    }
}
</script>
<template>
    <div class="background">
        <div class="container">
            <ul>
                <li v-for="(item, index) in  itemList ">
                    <img :src="item.icon" alt="foto">
                    <p>{{ item.name }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.background {
    background-color: #0282F9;
}

div {
    height: 150px;
    display: flex;
    align-items: center;

    ul {
        display: flex;
        align-items: center;
        width: 100%;

        li {
            display: flex;
            list-style-type: none;
            align-items: center;
            flex-grow: 1;

            img {
                width: 50px;
            }

            p {
                margin: 0px 20px;
                color: #fff;
            }
        }
    }
}
</style>