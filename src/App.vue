<template>
  <div id="app">
    <topSection />
    <middleSection />
    <bottomSection/>
  </div>
</template>

<script>
import topSection from './components/topSection.vue'
import middleSection from './components/middleSection.vue'
import bottomSection from './components/bottomSection.vue'

export default {
  components: {
    topSection,
    middleSection,
    bottomSection
  }
}
</script>

<style lang="sass" scoped>
#app 
  font-family: Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50

</style>
