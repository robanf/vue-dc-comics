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
    .immagini{

      width: calc(100% / 6 -20px) ;

      img{
        height: 250px;
        background-color: red;
        margin-right: 20px;
        margin-top:30px;
      }
    }
</style>