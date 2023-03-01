<template>
    <footer class="main-footer">
        <div class="footer-sidebar">
            <div class="container">
                <div class="card" v-for="item in sidebarItems">
                    <div class="card-img">
                        <img :src="item.img" alt="">
                    </div>
                    <div class="card-body">
                        <p>{{ item.text }}</p>
                    </div>
                </div>


            </div>

        </div>
        <div class="footer-links">
            <div class="container">
                <div class="row">
                    <div class="col">

                        <h2 class="menu-title ">dc comics</h2>
                        <ul class="menu">
                            <li class="menu-item" v-for="element in dcComics">{{ element }}</li>
                        </ul>


                        <h2 class="menu-title">shop</h2>
                        <ul>
                            <li class="menu-item" v-for="element in shop">{{ element }}</li>
                        </ul>

                    </div>
                    <div class="col">
                        <h2 class="menu-title">dc</h2>
                        <ul>
                            <li class="menu-item" v-for="element in dc">{{ element }}</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2 class="menu-title">sites</h2>
                        <ul>
                            <li class="menu-item" v-for="element in sites">{{ element }}</li>
                        </ul>
                    </div>


                </div>
                <div class="col">
                    <img src="/img/dc-logo-bg.png" alt="Dc Logo">
                </div>
            </div>
        </div>

        <div class="footer-social">

            <div class="container">
                <button class="btn btn-sign">sign-up now!</button>
                <div class="social-wrap">
                    <button class="btn btn-follow">follow us</button>
                    <ul class="social-icons">
                        <li v-for="icon in socialIcons"><img :src="icon" alt=""></li>
                    </ul>

                </div>
            </div>

        </div>
    </footer>
</template>
  
<script>
export default {
    data() {
        return {
            currentIndex: 0,
            sidebarItems: [
                {
                    img: '/img/buy-comics-digital-comics.png',
                    text: 'digital comics',
                },
                {
                    img: '/img/buy-comics-merchandise.png',
                    text: 'dc merchandise',
                },
                {
                    img: '/img/buy-comics-subscriptions.png',
                    text: 'subscription',
                },
                {
                    img: '/img/buy-comics-shop-locator.png',
                    text: 'comic shop locator',
                },
                {
                    img: '/img/buy-dc-power-visa.svg',
                    text: 'dc power visa',
                },
            ],
            socialIcons: [
                "/img/footer-facebook.png",
                "/img/footer-twitter.png",
                "/img/footer-youtube.png",
                "/img/footer-pinterest.png",
                "/img/footer-periscope.png"
            ],

            dcComics: [
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News'
            ],

            shop: [
                'Shop DC',
                'Shop DC Collectibles',
            ],
            dc: [
                'Terms Of Use',
                'Privacy policy (New)',
                'Ad Choices',
                'Advertising',
                'Privacy ',
                'Jobs',
                'Subscriptions',
                'Talent Workshops',
                'Subscriptions',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us',
            ],
            sites: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa ',
            ]

        }
    }

}
</script>
  
<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.main-footer {
    color: white;
}

.container {
    justify-content: space-between;
    padding: 10px;
    position: relative;
}

.footer-sidebar {
    background-color: $sidebar-bg;
    padding: 20px;
}

.card {
    padding: 20px;
    display: flex;
    align-items: center;
    gap: 10px;

    .card-img img {
        height: 40px;
    }

    &:last-child img {
        width: 40px;
    }

    .card-body {
        font-size: 10px;
        text-transform: uppercase;
    }

}

.footer-links {
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
    padding: 24px;
    color: white;
    overflow: hidden;

    .row {
        display: flex;
        gap: 15px;

        .menu {
            margin-bottom: 10px;
        }

        .menu-title {
            text-transform: uppercase;
            font-size: 15px;
            margin-bottom: 10px;
        }

        .menu-item {
            font-size: 12px;
            line-height: 14px;
            font-weight: 700;
            color: $link-color;
        }
    }
}


.col img {
    height: 400px;
    position: absolute;
    top: -75px;
    right: 0;

}

.footer-social {
    background-color: $footer-bg;
    padding: 20px;

    .btn {
        text-transform: uppercase;
        padding: 10px;
        font-weight: 700;
    }

    .btn-sign {
        background-color: unset;
        border: 2px solid $sidebar-bg;
        color: white;
        font-size: 12px;
    }

    .social-wrap {
        display: flex;
        align-items: center;
        gap: 20px;
    }

    .btn-follow {
        background-color: unset;
        color: $sidebar-bg;
        border: none;
    }

    .social-icons {
        display: contents;

        li img {
            height: 30px;
        }
    }
}
</style>