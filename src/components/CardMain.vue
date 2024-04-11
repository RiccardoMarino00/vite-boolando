<script>
export default{
    data(){
        return {
            currentIndex: 0,
            "products": [
            {
                "id": 1,
                "frontImage": "1.webp",
                "backImage": "1b.webp",
                "brand": "Levi's",
                "name": "Relaxed Fit",
                "price": 29.99,
                "isInFavorites": true,
                "badges": [
                    {
                        "type": "tag",
                        "value": "Sostenibilità"
                    },
                    {
                        "type": "discount",
                        "value": "-50%"
                    }
                ]
            },
            {
              "id": 2,
              "frontImage": "2.webp",
              "backImage": "2b.webp",
              "brand": "Guess",
              "name": "Roses Tee",
              "price": 20.99,
              "isInFavorites": true,
              "badges": [
                {
                  "type": "discount",
                  "value": "-30%"
                }
              ]
            },
            {
              "id": 3,
              "frontImage": "3.webp",
              "backImage": "3b.webp",
              "brand": "Come Zucchero Filato",
              "name": "Voglia di colori pastello",
              "price": 129.99,
              "isInFavorites": false,
              "badges": [
                {
                  "type": "discount",
                  "value": "-30%"
                }
              ]
            },
            {
              "id": 4,
              "frontImage": "4.webp",
              "backImage": "4b.webp",
              "brand": "Levi's",
              "name": "Tee Unisex",
              "price": 14.99,
              "isInFavorites": false,
              "badges": [
                {
                  "type": "tag",
                  "value": "Sostenibilità"
                },
                {
                  "type": "discount",
                  "value": "-50%"
                }
              ]
            },
            {
              "id": 5,
              "frontImage": "5.webp",
              "backImage": "5b.webp",
              "brand": "Maya Deluxe",
              "name": "Stripe Bodice",
              "price": 99.99,
              "isInFavorites": true,
              "badges": [
                {
                  "type": "tag",
                  "value": "Sostenibilità"
                },
                {
                  "type": "discount",
                  "value": "-50%"
                }
              ]
            },
            {
              "id": 6,
              "frontImage": "6.webp",
              "backImage": "6b.webp",
              "brand": "Esprit",
              "name": "Maglione - Black",
              "price": 29.99,
              "isInFavorites": true,
              "badges": [
                {
                  "type": "tag",
                  "value": "Sostenibilità"
                }
              ]
            }
           ]
         }
    },

}
</script>

<template>
<div class="col-4" v-for="(product, i) in products" :key="i">
    <div class="card">
        <div class="card-header">
            <img :src="product.frontImage" alt="">
            <div v-for="(badge, i) in products[currentIndex].badges">
                <span class="sconto"></span>
                <span class="eco-friendly"></span>
            </div>
            
            <span class="cuore">&hearts;</span>
            <img class="overlay " :src="product.backImage"></img>
        </div>
        <div class="card-body">
            <p class="littlegray">{{ product.brand }}</p>
            <h3>{{ product.name }}</h3>
            <p>
                <span class="prize-red">&euro;</span>
                <span class="text-line">{{product.price}}&euro;</span>
            </p>
        </div>
    </div>
</div>
</template>

<style>
</style>