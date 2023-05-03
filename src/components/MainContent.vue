<script>
export default {
    name: 'MainContent',
    data() {
        return {
            listComics: [
                {
                    name: 'Charcters',
                    visible: false,
                }, {
                    name: 'Comics',
                    visible: false,
                },
                {
                    name: 'Movies',
                    visible: false,
                },
                {
                    name: 'TV',
                    visible: false,
                },
                {
                    name: 'Games',
                    visible: false,
                },
                {
                    name: 'Videos',
                    visible: false,
                }, {
                    name: 'News',
                    visible: false,
                },
            ],
            listShop: [
                {
                    name: 'Shop DC',
                    visible: false,
                }, {
                    name: 'Shop DC Collectibles',
                    visible: false,
                }
            ],
            listDC: [
                {
                    name: 'Terms Of Use',
                    visible: false,
                },
                {
                    name: 'Privacy policy (New)',
                    visible: false,
                },
                {
                    name: 'Add Choices',
                    visible: false,
                },
                {
                    name: 'Advertising',
                    visible: false,
                },
                {
                    name: 'Jobs',
                    visible: false,
                },
                {
                    name: 'Subscriptions',
                    visible: false,
                },
                {
                    name: 'Talent Workshops',
                    visible: false,
                },
                {
                    name: 'CPSC Certificates',
                    visible: false,
                },
                {
                    name: 'Ratings',
                    visible: false,
                },
                {
                    name: 'Shop Help',
                    visible: false,
                },
                {
                    name: 'Contact Us',
                    visible: false,
                },
            ],
            listSites: [
                {
                    name: 'DC',
                    visible: false,
                },
                {
                    name: 'MAD Magazine',
                    visible: false,
                },
                {
                    name: 'DC Kids',
                    visible: false,
                },
                {
                    name: 'DC Universe',
                    visible: false,
                },
                {
                    name: 'DC Power Visa',
                    visible: false,
                },
            ]
        }
    }
}
</script>
<template>
    <div class="background">
        <div class="container d-flex justify-content-between">
            <div class="lists">
                <!-- ------- -->
                <div class="comics-shop">
                    <ul>
                        <li>
                            <h2>DC COMICS</h2>
                        </li>
                        <li v-for="(item, index) in listComics" :key="index"><a href="#">{{ item.name }}</a></li>
                    </ul>
                    <!-- --------- shop-->
                    <ul>
                        <li>
                            <h2>SHOP</h2>
                        </li>
                        <li v-for="(item, index) in listShop" :key="index"><a href="#"> {{ item.name }}</a></li>
                    </ul>
                </div>
                <!-- ---------- -->
                <div class="list-dc">
                    <ul>
                        <li>
                            <h2>DC</h2>
                        </li>
                        <li v-for="(item, index) in listDC" :key="index"><a href="#">{{ item.name }}</a></li>
                    </ul>
                </div>
                <!-- ------- -->
                <div class="list-sites">
                    <ul>
                        <li>
                            <h2>SITES</h2>
                        </li>
                        <li v-for="(item, index) in listSites" :key="index"><a href="#">{{ item.name }}</a></li>
                    </ul>
                </div>

            </div>
            <div class="logo">
                <img src="../../public/img/dc-logo-bg.png" alt="foto">
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.background {
    background-image: url(../..//public/img/footer-bg.jpg);
    background-size: cover;
    overflow-y: hidden;
}

img {
    transform: scale(1.2);
}

ul {
    li {
        padding: 5px 0px;
        padding-right: 15px;

        h2 {
            color: #fff;
        }

        a {
            color: #fff;
            text-decoration: none;
            list-style-type: none;
            letter-spacing: 1px;
            font-weight: 100;
        }
    }
}

.lists {
    display: flex;
    padding-top: 20px;
}
</style>