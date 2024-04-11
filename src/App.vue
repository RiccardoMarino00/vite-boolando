<script>
import headerBoo from './components/Header.vue';
import mainBoo from './components/Main.vue';
import footerBoo from './components/Footer.vue';

export default {
  data(){
    return{
      message: 'ciao'
    }
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
