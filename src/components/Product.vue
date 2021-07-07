<template>
  <div>
      <main>
          <h1>--STIAMO LAVORANDO PER VOI--</h1>
          <div class="container">

          <div class="pippo">
                <Prodcard
                v-for="(item,index) in links" 
                :key="index"
                :prod="item"/>
            </div>
          </div>
            
            
          
      </main>
  </div>
</template>

<script>
import Prodcard from '@/components/Prodcard.vue'
import array from '@/data/array.js'
export default {
    name:"product",
    components:{
        Prodcard,
    },
     data(){
        return{
         links:array
        }
    }
}
</script>

<style lang="scss" scoped>
    main{
        color: white;
        background-color: black;
        h1{
            color: white;
            line-height: 100px;
        }
        .container{
            width: 1080px;
            margin: auto;

            .pippo{

                display: flex;
                justify-content: space-around;
                flex-wrap:wrap;
                width: 100%;
            }
        }
    }
</style>