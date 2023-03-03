<template>
    <footer class="main-footer">
        <div class="sidebar">
            <div class="container">
                <AppSidebar v-for="item in sidebarItems" :key="item.text" :text="item.text" :img="item.img" />
            </div>
        </div>
        <div class="footer-links">
            <div class="container">
                <div class="row">
                    <Menu v-for="item in menuLinks" :key="item.title" :links="item.links" :title="item.title" />

                </div>
                <div class="col">
                    <img src="/img/dc-logo-bg.png" alt="Dc Logo">
                </div>
            </div>
        </div>

        <div class="footer-social">

            <div class="container">
                <button class="btn btn-outline">sign-up now!</button>
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
import AppSidebar from './AppSidebar.vue';
import Menu from './Menu.vue'
export default {
    components: {
        AppSidebar,
        Menu,
    },
    data() {
        return {
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
            menuLinks: [
                {
                    title: 'dc comics',
                    links: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Collectibles',
                        'Videos',
                        'Fans',
                        'News']

                },
                {
                    title: 'dc',
                    links: [
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
                        'Contact Us',]

                },
                {
                    title: 'sites',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa ',]

                },
                {
                    title: 'shop',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles',]

                },
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

.sidebar {
    background-color: $sidebar-bg;
    padding: 20px;
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
        gap: 40px;
        position: relative;
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

    .btn-outline {

        background-color: unset;
        border: 2px solid $sidebar-bg;
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