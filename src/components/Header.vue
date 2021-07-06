<template>
  <div>
      <header>
      <a href="#">
          <img src="@/assets/img/dc-logo.png" alt="">
      </a>

      <nav>
          <ul>
              <li v-for="(link,index) in links" :key="index">
                  <a href="link.url" :class="{active: link.current}">{{link.text}}</a>
              </li>
          </ul>
      </nav>
      </header>
  </div>
</template>

<script>
export default {
    name:'Header',
    data(){
        return{
            links:[
                {
                    text:'Character',
                    url:'#',
                    current:false
                },
                 {
                    text:'Comic',
                    url:'#',
                    current:true
                },     
                {
                    text:'movies',
                    url:'#',
                    current:false
                },
                {
                    text:'tv',
                    url:'#',
                    current:false
                },
                {
                    text:'games',
                    url:'#',
                    current:false
                },
                {
                    text:'collectibles',
                    url:'#',
                    current:false
                },
                {
                    text:'video',
                    url:'#',
                    current:false
                },
                {
                    text:'fans',
                    url:'#',
                    current:false
                },
                {
                    text:'news',
                    url:'#',
                    current:false
                },
                {
                    text:'shop',
                    url:'#',
                    current:false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
header{
    height: 80px;
    text-align: center;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: white;
    a{
        width: 50%;
        img{
            height: 80px;
            width: auto;
        }
    }
    ul{
        list-style: none;
        display: flex;
        justify-content: start;
        margin-right:120px;

        li{
            margin: 10px;
            display: inline-block;
            font-size: $font-primary;
            text-transform: uppercase;
            font-weight: bold;
            a{
                text-decoration: none;
                color: black;
                &:hover,
                &.active{
                    color: blue;
                    border-bottom: 5px solid blue;
                    padding-bottom:30px ;
                }
            }

        }
    }
}
</style>