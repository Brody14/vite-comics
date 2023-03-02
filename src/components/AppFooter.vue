<template>
    <footer class="main-footer">
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
                <button class="btn-sign">sign-up now!</button>
                <div class="social-wrap">
                    <ul class="social-icons">
                        <li class="follow">follow us</li>
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
                'TV',
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
            font-size: 10px;
            line-height: 15px;
            font-weight: 700;
            color: $link-color;
        }
    }
}

.col {
    margin-bottom: 10px;
}

.col img {
    height: 475px;
    position: absolute;
    top: -112px;
    right: 0;

}

.footer-social {
    background-color: $footer-bg;
    padding: 10px;

    .btn-sign {
        text-transform: uppercase;
        padding: 10px;
        font-weight: 700;
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

    .follow {
        color: $sidebar-bg;
        text-transform: uppercase;
        font-size: 15px;
        font-weight: 700;
    }

    .social-icons {
        display: contents;

        li img {
            height: 30px;
        }
    }
}
</style>