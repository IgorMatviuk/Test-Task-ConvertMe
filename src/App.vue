<template>
  <div id="app">
    <Header/>
    <Main />
    <Careers />
    <Tabs/>
    <Carousel/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Careers from './components/Careers.vue'
import Tabs from './components/Tabs.vue'
import Carousel from './components/Carousel.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Careers,
    Tabs,
    Carousel,
    Footer
  }
}
</script>

<style lang="scss">

</style>
