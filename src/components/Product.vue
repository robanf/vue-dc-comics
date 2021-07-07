<template>
  <div>
      <main>
          
          <div class="jumbo"></div>
          <div class="container">
            <div class="btn">CURRENT SERIES</div>
          <div class="pippo">
                <Prodcard
                v-for="(item,index) in links" 
                :key="index"
                :prod="item"/>
            </div>
            <div class="btn load">LOAD MORE</div>
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
        .jumbo{
            background-image: url("../assets/img/jumbotron.jpg");
            height: 300px;
            background-size:cover ;
        }
        .btn{
            display: inline-block;
            padding: 10px;
            border: 1px solid blue;
            background-color: blue;
            font-weight: bold;
        }
        .load{
            text-align: center;
            margin-left:45% ;
            margin-bottom: 20px;
        }
        .container{
            width: 1080px;
            margin: auto;
            background-color: black;

            .pippo{

                display: flex;
                flex-wrap:wrap;
                width: 100%;
            }
        }
    }
</style>