<template>
  <div class="Prodotti">
      <div class="immgagini">
        <img :src="prod.thumb" alt="">
         <div>{{prod.series}}</div>
      </div>
  </div>
</template>

<script>
export default {
    name:'Prodcard',
    props:["prod"]
}
</script>

<style lang="scss" >
  .Prodotti{
    width: calc(100% / 6 ) ;
    border: 15px solid black;
  }
    .immagini{

      
      height: 250px;
        background-color: red;
        margin-top:30px;

      img{
       height: 100%;
      }
    }
</style>