<script>
import cardsData from '../db.json'
export default {
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
    components: {
        cardsData,
    }
}
</script>


<template>
    <main>
        <section class="main">
            <div class="container">
                <div class="row">
                    <div class="col-4" v-for="(product, i) in products" :key="id">
                        <div class="card">
                            <div class="card-header">
                                <img :src="product.frontImage" alt="">
                                <div v-for="(badge, i) in products[currentIndex].badges">
                                    <span class="sconto"></span>
                                    <span class="eco-friendly"></span>
                                </div>
                                
                                <span class="cuore">&hearts;</span>
                                <div class="overlay relaxed"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">{{ product.brand }}</p>
                                <h3>{{ product.name }}</h3>
                                <p>
                                    <!-- <span class="prize-red">&euro;</span> -->
                                    <span class="text-line">{{product.price}}&euro;</span>
                                </p>
                            </div>
                        </div>
                    </div>
    
                    <!-- <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/2.webp" alt="">
                                <span class="sconto">-30%</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay guess"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Guess</p>
                                <h3>Roses Tee</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/3.webp" alt="">
                                <span class="sconto">-30%</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay zucchero"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Come Zucchero Filato</p>
                                <h3>Voglia di colori pastello</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/4.webp" alt="">
                                <span class="sconto">-50%</span>
                                <span class="eco-friendly">Sostenibilità</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay levis"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Levi's</p>
                                <h3>Tee unisex</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/5.webp" alt="">
                                <span class="cuore">&hearts;</span>
                                <div class="overlay maya"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Maya Deluxe</p>
                                <h3>Stripe bodice</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>
                            </div>
                        </div>
                    </div>
    
                    <div class="col-4">
                        <div class="card">
                            <div class="card-header">
                                <img src="/public/6.webp" alt="">
                                <span class="eco-friendly-woman">Sostenibilità</span>
                                <span class="cuore">&hearts;</span>
                                <div class="overlay espirit"></div>
                            </div>
                            <div class="card-body">
                                <p class="littlegray">Esprit</p>
                                <h3>Maglione-Black</h3>
                                <p><span class="prize-red">14,99&euro;  </span><span class="text-line">29,99&euro;</span></p>   
                            </div>
                        </div>
                    </div>        -->
                </div>
            </div>
        </section>
    </main>

</template>