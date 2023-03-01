<template>
    <header class="main-header">
        <div class="container">
            <figure>
                <img class="header-logo" src="/img/dc-logo.png" alt="DC logo">
            </figure>

            <nav class="main-nav">
                <ul class="nav">
                    <li class="nav__item">LINK</li>
                    <li class="nav__item active">LINK</li>
                    <li class="nav__item">LINK</li>
                    <li class="nav__item">LINK</li>
                    <li class="nav__item ">LINK</li>
                    <li class="nav__item">LINK</li>
                    <li class="nav__item">LINK</li>
                    <li class="nav__item">LINK</li>
                    <li class="nav__item">LINK</li>
                    <li class="nav__item">LINK</li>
                </ul>
            </nav>

        </div>

    </header>
</template>
  
<script>

</script>
  
<style scoped>
.container {
    align-items: center;
    justify-content: space-between;
}

.main-header {
    padding: 25px;
    position: relative;
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
}

.nav__item:active,
.nav__item.active,
.nav__item:hover {
    color: #0282f9;
}

.nav__item:active::after,
.nav__item.active::after {
    content: '';
    display: block;
    height: 5px;
    width: 40px;
    background-color: #0282f9;
    position: absolute;
    bottom: 0;
}
</style>