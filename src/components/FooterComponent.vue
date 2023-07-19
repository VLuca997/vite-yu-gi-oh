<script>
// my-component.js
export default {
    data() {
        return 
    },
}
</script>

<template >
    <div class="footer">
        <div>
            <div class="footer-col"></div>
            <div class="footer-col"></div>
            <div class="footer-col"></div>
        </div>
        <div>
            <div class="footer-col"></div>
            <div class="footer-col"></div>
            <div class="footer-col"></div>

        </div>
        <div>
            <div class="footer-col"></div>
            <div class="footer-col"></div>
            <div class="footer-col"></div>

        </div>
    </div>
</template>

<style lang="scss" >
    .footer{
        display: flex;
        justify-content: center;
        flex-direction: row;
        padding: 50px;  

        
        
    }
    .footer-col:first-child{
            justify-content: flex-end;
            background-color: blue;
        }
    .footer-col{
        width: 150px;
        height: 150px;
        background-color: red;
        border: 2px dashed green;

    }
    

</style>