<template>
  <div id="app">
    <Jumbotron/>
    <WhyC/>
    <WhyJ/>
    <Info/>
    <Levels/>
    <Footer/>
  </div>
</template>

<script>
import Jumbotron from './components/Jumbotron.vue'
import WhyC from './components/WhyC.vue'
import WhyJ from './components/WhyJ.vue'
import Info from './components/Info.vue'
import Levels from './components/Levels.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Jumbotron,
    WhyC,
    WhyJ,
    Info,
    Levels,
    Footer
  }
}
</script>

<style lang="scss">

</style>
