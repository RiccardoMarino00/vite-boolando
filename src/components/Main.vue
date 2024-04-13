<script>
import dataCard from '../assets/db.json'
import card from './CardMain.vue'
export default {
    data(){
        return {
            products: dataCard.products
         }
    },
    
    components: {
        card,
    }
}
</script>


<template>
    <main>
        <section class="main">
            <div class="container">
                <div class="row">
                    <div class="col-4" v-for="(product, i) in products" :key="i">
                      <card :product="product"/>
                        <!-- <div class="card">
                            <div class="card-header">
                                <img :src="product.frontImage" alt="">
                                <ul >
                                    <li v-for="(badge, i) in product.badges" :class="`badge--${badge.type}`" :key="i">{{ badge.value }}</li>
                                </ul>
                                
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
                        </div> -->
                    </div>

                        <!-- <card/> -->
                    <!-- <div class="col-4">
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
                    </div> -->
                </div>
            </div>
        </section>
    </main>

</template>