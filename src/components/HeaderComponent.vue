<script>
// my-component.js
export default {
  data() {
    return 
  },
}
</script>

<template>
  <div>
    
      <header>

        <h1>TEMPLATE BASE HEADER</h1>
        <h2>TEST VARIABLES.SCSS </h2>

    </header>
  </div>
</template>

<style lang="scss" >
@import "/src/assets/scss/main.scss"; // import di main tramite le variabili di variables.scss
div{
  
  border: 2px dashed black;
  align-content: center;
  
  
  header{
    align-items: center;
    display: flex;
    justify-content: center;
    padding: 100px;
    h1{
      padding: 3.125rem;
      background-color: lightgray;
      border-radius: 20px;
      
    }
  }
}
</style>