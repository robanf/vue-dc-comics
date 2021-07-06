<template>
  <div>
      <header>
      <a href="#">
          <img src="@/assets/img/dc-logo.png" alt="">
      </a>

      <nav>
          <ul>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
              <li><a href="#">ciao sono mario</a></li>
          </ul>
      </nav>
      </header>
  </div>
</template>

<script>
export default {

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
        width: 80%;
        list-style: none;
        display: flex;
        justify-content: start;

        li{
            margin: 10px;
            display: inline-block;
            font-size: $font-primary;
            a{
                text-decoration: none;
                color: black;
            }
        }
    }
}
</style>