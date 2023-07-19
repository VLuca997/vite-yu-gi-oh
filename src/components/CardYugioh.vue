<script>
    // my-component.js
export default {
    data() {
        return {
            
        }
    },
    components:{
        cardYuGiOh:[]
    },
    props:{
      cards: {
        this: Array,
        default: []
      }
    },
}   
</script>


<template>

    <div class="container-fluid mt-4 d-flex flex-wrap">
        <div class="row  text-center"
            v-for="(cards, i) in cards" :key="i.id" >


            <div class="cotainer-fluid" v-if="i < 15">
                <div class="card-container" >
                    <div class="img-container">
                        
                        <img class="img-fluid" :src="cards.card_images[0].image_url" alt="">

                    </div>
                    <div class="content">
                        <p>{{ cards.name }}</p>
                        <p>{{ cards.type }}</p>
                    </div>
                </div>
            </div>

            


        </div>
    </div>

</template>



<style lang="scss" scoped>
.container-fluid {
    max-width: 1200px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  flex-basis: 20%;
}


</style>