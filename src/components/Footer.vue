<template>
  <div>
      <footer>
          <div class="shop">
              <ul>
                  <li  v-for="(shop,index) in shops" :key="index">
                      <a href="#">
                          <img :src="require('@/assets/img/buy-comics-'+ shop.name )" alt="">

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
                },
                {
                    name:'merchandise.png',
                },
                {
                    name:'shop-locator.png',
                },
                {
                    name:'subscriptions.png',
                },
                {
                    name:'power-visa.svg',
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

                        img{
                            height: 80%;
                            display: inline-block;
                        }
                    }
                }
            }
        }
    }
</style>