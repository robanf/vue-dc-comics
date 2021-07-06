<template>
  <div id="app">
 <!--    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Header/>
    <main>
        <Product/>
    </main>
    <Footer/>
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */
import Header from './components/Header.vue'
import Product from './components/Product.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
/*     HelloWorld, */
    Header,
    Product,
    Footer
  }
}
</script>

<style lang="scss">
@import 'style/commons.scss';

</style>
