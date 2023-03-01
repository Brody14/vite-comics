<template>
    <div class="sidebar">
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
</template>
  
<script>
export default {
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
            ]
        }
    }
}

</script>
  
<style lang="scss" scoped>
@use '../style/partials/variables' as *;


.container {
    justify-content: space-between;
    padding: 10px;
}

.sidebar {
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
        color: white;
    }

}
</style>