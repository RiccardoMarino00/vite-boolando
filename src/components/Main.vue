<script>
// import dataCard from '/ProgettiBoolean/vite-boolando/db.json'
import card from './CardMain.vue'
import {store} from '../store'
export default {
    data(){
        return {
            // products: dataCard.products,
            store,
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
                    <div class="col-4" v-for="(product, i) in store.products" :key="i">
                      <card :product="product"/>
                    </div>
                </div>
            </div>
        </section>
    </main>

</template> 






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