<script>
// my-component.js
export default {
    data() {
    return 
    },
}
</script>
<template>
    <div class="container-generale">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>     
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>   
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>

            
    </div>
</template>
<style lang="scss" scoped>

.container-generale{
    padding: 50px;
    display: flex;
    justify-content: space-around;
    flex-direction: row;
    flex-wrap: wrap;
}
.item{
    height: 100px;
    width: 100px;

}
.item:nth-child(even){
    background-color: red;
    
}
.item:nth-child(odd){
        background-color: blue;
}   

</style>