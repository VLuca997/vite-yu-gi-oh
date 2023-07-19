<script >
//import component h1
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';


// my-component.js
export default {
  data() {
    return 
  },
  components:{
    HeaderComponent, MainComponent, FooterComponent
  }
}
</script>

<template>
    <HeaderComponent />
    <MainComponent/>
    <FooterComponent />
</template>

<style scoped>

</style>
