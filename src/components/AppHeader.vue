<template>
    <header class="main-header">
        <div class="container">
            <figure>
                <img class="header-logo" src="/img/dc-logo.png" alt="DC logo">
            </figure>

            <nav class="main-nav">
                <ul class="nav">
                    <li class="nav__item" v-for="item in navbarItems"> {{ item }}</li>

                </ul>
            </nav>

        </div>

    </header>
</template>
  
<script>
export default {
    data() {
        return {
            navbarItems: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop']
        }
    }

}


</script>
  
<style scoped>
.container {
    align-items: center;
    justify-content: space-between;
}

.main-header {
    padding: 25px;
}

.header-logo {
    height: 50px;
}

.nav {
    display: flex;
    gap: 10px;
}

.nav__item {
    cursor: pointer;
    padding: 5px;
    text-transform: uppercase;
    font-size: 12px;
    position: relative;
}

.nav__item:active,
.nav__item:hover {
    color: #0282f9;
}

.nav__item:active::after {
    content: '';
    display: block;
    height: 4px;
    width: 100%;
    background-color: #0282f9;
    position: absolute;
    bottom: -37px;
    left: 0;
    right: 0;
}
</style>