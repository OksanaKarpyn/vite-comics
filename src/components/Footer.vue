<script>
export default {
    name: 'Footer',
    data() {
        return {
            listIcon: [
                {
                    icon: '../../public/img/footer-facebook.png',
                    visible: false
                },
                {
                    icon: '../../public/img/footer-twitter.png',
                    visible: false
                },
                {
                    icon: '../../public/img/footer-youtube.png',
                    visible: false
                },
                {
                    icon: '../../public/img/footer-pinterest.png',
                    visible: false
                },
                {
                    icon: '../../public/img/footer-periscope.png',
                    visible: false
                },
            ]
        }
    }
}
</script>
<template>
    <div class="background">
        <div class="container d-flex justify-content-between align-items-center py-4">
            <div>
                <button class="btn btn-outline-primary text-white">SIGN-UP NOW!</button>
            </div>
            <div class="list-footer">
                <ul>
                    <li>
                        <h2>FOLLOW US</h2>
                    </li>
                    <li v-for="(item, index) in  listIcon " :key="index">
                        <a href="#"><img :src="item.icon" alt="icon"></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.background {
    background-color: #303030;
}

ul {
    display: flex;
    align-items: center;
    list-style-type: none;
    margin-bottom: 0px;

    li {
        padding: 0px 10px;

        h2 {
            color: #0282F9;
            font-size: 1.2rem;
        }

        a {
            img {}
        }
    }
}

.list-footer {}
</style>
