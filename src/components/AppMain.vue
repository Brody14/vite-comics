<template>
    <main class="main-content">

        <div class="container">
            <span class="btn btn-blue badge">current series</span>
            <div class="grid">
                <Card v-for="(comic, i) in comics" :key="i" :thumb="comic.thumb" :series="comic.series" />

            </div>

        </div>
        <div class="container">
            <button class="btn btn-blue">load more</button>
        </div>
    </main>
</template>
  
<script>
import Card from './Card.vue'

export default {
    components: {
        Card,
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.brooklyncomicshop.com/BCS/wp-content/uploads/2019/02/Action-Comics-419-Brooklyn-Comic-Shop.jpg.jpeg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1INJU012ISBN_0.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1dcmh033isbn_0.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/dcdcea88706ab1684584701c5b27598d/M/1/M1REHC036ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BATM067_0.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/dcdcea88706ab1684584701c5b27598d/M/1/M1BTMA028ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/dcdcea88706ab1684584701c5b27598d/M/1/M1BTMA010_0.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1OMEG008ISBN_0.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1blin005isbn_0_etb5tnzfio9togjg.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA014ISBN_0.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/dcdcea88706ab1684584701c5b27598d/M/1/M1BLLA027ISBN_0.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}

</script>
  
<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.main-content {
    background-color: $main-bg;
    padding: 20px;
    color: white;
}

.container {
    position: relative;
}

.container+.container {
    justify-content: center;
}

.grid {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    gap: 30px;
    padding: 20px 10px;
    margin-bottom: 30px;
}

.btn-blue {
    text-align: center;
    background-color: $sidebar-bg;
    border: none;
    width: 17%;
}

.btn-blue.badge {
    font-size: 20px;
    position: absolute;
    top: -40px;
}
</style>