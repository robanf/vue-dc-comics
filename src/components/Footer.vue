<template>
  <div>
      <footer>
          <div class="shop">
              <ul>
                  <li  v-for="(shop,index) in shops" :key="index">
                      <a href="#">
                          <img :src="require('@/assets/img/buy-comics-'+ shop.name )" alt="">
                            <span>{{shop.descrizione}}</span>
                        </a>
                    </li>

              </ul>
          </div>
      </footer>
  </div>
</template>

<script>
export default {
    name:'Footer',
    data(){
        return{
            shops:[
                {
                    name:'digital-comics.png',
                    descrizione:'digital comics',
                },
                {
                    name:'merchandise.png',
                    descrizione:'dc merchandise',
                },
                {
                    name:'shop-locator.png',
                    descrizione:'comic shop locator',
                },
                {
                    name:'subscriptions.png',
                    descrizione:'subscriptions',
                },
                {
                    name:'power-visa.svg',
                    descrizione:'dc power visa',
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    footer{
        .shop{
            height: 150px;
            background-color: blue;
            ul{
                display: flex;
                justify-content: space-evenly;
                align-items: center;
                height: 100%;
                li{
                    height: 100px;
                    width: auto;
                    display: inline-block;
                    a{
                        height: 100%;
                        display: flex;
                        align-items: center;
                        text-decoration: none;
                        img{
                            height: 70%;
                            display: inline-block;
                            margin: 5px;
                        }
                        span{
                            color: white;
                            font-size: 16px;
                            text-transform: uppercase;
                        }
                    }
                }
            }
        }
    }
</style>