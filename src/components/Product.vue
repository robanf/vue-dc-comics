<template>
  <div>
      <main>
          <h1>--STIAMO LAVORANDO PER VOI--</h1>
            <Prodcard
            v-for="(item,index) in links" 
            :key="index"
            :prod="item"/>
            
          
      </main>
  </div>
</template>

<script>
import Prodcard from '@/components/Prodcard.vue'
import Pippo from '@/components/Pippo.vue'
import array from '@/data/array.js'
export default {
    name:"product",
    component:{
        Prodcard,
        Pippo
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
        
        background-color: black;
        h1{
            color: white;
            line-height: 100px;
        }
        ul{
            display: flex;
            justify-content: space-evenly;
            li{
                display: inline-block;
                margin: 20px 0px;
                color: white;
                text-align: center;
                .fumetto{
                    background-color: green;
                    height: 150px;
                    width: 150px;
                }

            }
        }
    }
</style>