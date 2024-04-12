<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import { store } from './store';
import axios from 'axios';


export default{
  data(){
    return{
      store
    }
  },
  components:{
    AppHeader,
    AppMain,
    AppFooter
  },
  methods:{
    fetchProducts(){
      axios.get('https://www.mamma.com/posts')
      .then((res)=>{

        console.log(res)
      })
      
    }
  },
  created(){
    this.fetchProducts()
  }
}

</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>

</template>


<style lang="scss">
@use './style/general';




</style>

