<script>
import headerBoo from './components/Header.vue';
import mainBoo from './components/Main.vue';
import footerBoo from './components/Footer.vue';
import axios from 'axios'
import {store} from './store.js'

export default {
  data(){
    return{
      message: 'ciao'
    }
  },
  methods: {
    fetchProducts(){
      axios.get('http://localhost:3000/products').then((res) => {
        console.log(res.data)
        store.products = res.data
      })
    }

  },
  created (){
    this.fetchProducts()
  },
  mounted(){
    console.log('mounted')
  },
  components:{
    headerBoo,
    mainBoo,
    footerBoo,
  }
}
</script>

<template>
 <body class="debug">
    <headerBoo />
    <mainBoo />
    <footerBoo />  
</body>
</template>

<style lang="scss">
@use './style/general';

</style>
