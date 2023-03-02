<template>
    <div class="card">
        <div class="card-img">
            <img :src="img" alt="">
        </div>
        <div class="card-body">
            <p>{{ text }}</p>
        </div>
    </div>
</template>
  
<script>
export default {
    props: {
        img: {
            type: String,
            required: true
        },
        text: {
            type: String,
            required: true
        }
    }
}

</script>
  
<style lang="scss" scoped>
@use '../style/partials/variables' as *;

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