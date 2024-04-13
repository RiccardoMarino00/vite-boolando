<script>
import badge from './BadgeCard.vue'
export default{
  props: ['product'],
  components: {
    badge,
  }
}
    
     



</script>

<template>
                        <div class="card">
                            <div class="card-header">
                                <img :src="product.frontImage" alt="">
                                <ul >
                                    <badge v-for="(badge, i) in product.badges" :key="i" :text="badge.value"  :type="badge.type" />
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
                        </div>

</template>

<style>
</style>