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
          <div>
              
          </div>
          <div class="last-link">
              <div>
                        <div class="colonne-link">
                            <h3>DC COMICS</h3>
                            <ul>
                                <li>roba a caso</li>
                                <li>roba a caso</li>
                                <li>roba a caso</li>
                                <li>roba a caso</li>
                                <li>roba a caso</li>
                                <li>roba a caso</li>
                            </ul>
                            <h3>SHOP</h3>
                            <ul>
                                <li>shop dc</li>
                                <li>shop dc collezionabile</li>
                            </ul>
                        </div>
                        <div class="colonne-link">
                            <h3>DC</h3>
                            <ul>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                                <li> robe dc</li>
                            </ul>
                        </div>
                    <div class="colonne-link">
                        <h3>SITES</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC kids</li>
                            <li>DC universe</li>
                            <li>DC Power visa</li>
                        </ul>
                    </div>
                </div>

                <div class="imgDC"></div>
            </div>

                <div class="social-media">
                    <div>
                        <a href="#">ISCRIVITI ORA</a>
                    </div>
                    <div class="link-social">
                        <ul>
                            <li>Follow us</li>
                            <li> <img src="@/assets/img/footer-facebook.png" alt="">  </li>
                            <li><img src="@/assets/img/footer-periscope.png" alt=""></li>
                            <li><img src="@/assets/img/footer-pinterest.png" alt=""></li>
                            <li><img src="@/assets/img/footer-twitter.png" alt=""></li>
                            <li><img src="@/assets/img/footer-youtube.png" alt=""></li>
                        </ul>
                    </div>
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
        .last-link{
            background-image: url("../assets/img/footer-bg.jpg");
            display: flex;
            justify-content: space-around;
            height: 300px;
            .colonne-link{
                display: inline-block;
                margin: 0 20px;
                color: white;
                ul{
                    margin: 20px;
                }
            }
            .imgDC{
                height: 300px;
                width: 300px;
                background-image: url("../assets/img/dc-logo-bg.png");
                background-size:cover ;
            }
        }
        .social-media{
            background-color: rgb(22, 22, 22);
            height: 110px;
            display: flex;
            justify-content: space-around;
            align-items: center;
            a{
                color: white;
                text-decoration: none;
                padding: 10px;
                font-weight: bold;
                border: 2px solid blue;
            }
            .link-social{
                    color: blue;
                    font-weight: bold;
                    ul{
                        display: flex;
                        align-items: center;
                        
                        li{
                            display: inline-block;
                            margin: 0 10px;
                        }
                    }
            }
        }
    }
</style>