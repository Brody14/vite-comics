<template>
    <div class="card">
        <img :src="thumb" alt="">
        <h2>{{ series }}</h2>
    </div>
</template>

<script>
export default {
    props: {
        thumb: {
            type: String,
            required: true
        },
        series: {
            type: String,
            required: true
        }
    }
}

</script>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.card {
    text-transform: uppercase;
    font-size: 8px;

    h2 {
        font-weight: 100;
    }
}

.card img {
    height: 170px;
    aspect-ratio: 1/1;
    margin-bottom: 20px;
}
</style>