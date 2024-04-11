<script>
import cardsData from '../db.json'
import card from './CardMain.vue'
export default {
    
    components: {
        cardsData,
        card,
    }
}
</script>


<template>
    <main>
        <section class="main">
            <div class="container">
                <div class="row">
                    <card/>
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