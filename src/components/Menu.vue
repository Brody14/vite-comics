<template>
    <div class="col">

        <h2 class="menu-title ">{{ title }}</h2>
        <ul class="menu">
            <li class="menu-item" v-for="(link, i) in links" :key="i">{{ link }}</li>
        </ul>

    </div>
</template>

<script>
export default {
    props: {
        title: {
            type: String,
            required: true
        },
        links: {
            type: Array,
            required: true
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.col:nth-child(4n) {
    position: absolute;
    bottom: -16px;
}

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
</style>

