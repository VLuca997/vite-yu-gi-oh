<script >
//import component h1
import CardYugioh from './components/CardYugioh.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import ImputComponent from './components/ImputComponent.vue'
import axios from 'axios'


// my-component.js
export default {
    components:{
      CardYugioh,HeaderComponent,ImputComponent
    },
    data() {
      return {
        cards:[]
      }
    },
    created() {
      axios
      .get('https://db.ygoprodeck.com/api/v7/cardinfo.php')
      .then(response =>{  
        this.cards = response.data.data;
        
        console.log(response.data.data);
      })
      .catch(error => {
        console.error(error);
      });
      
    },
};
</script>

<template>
  <div class="container-xl">
    <HeaderComponent />
    <ImputComponent />
    <CardYugioh :cards="cards"/>
  </div>


</template>


<style lang="scss" >
//importo  da main.scss l'scss e css di bootstrap
@use "assets/scss/main";

</style>
