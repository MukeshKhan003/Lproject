<template>
  <div id="app">
    <FHeader :header_name="header_name"/>
    <Fworld />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Fworld from './components/Fworld.vue'
import FHeader from './components/FHeader.vue'

export default {
  name: 'App',
  components: {
    Fworld,
    FHeader
  },
  data(){
    return({
      header_name: 'என் கண்மணிக்காக 🖤'
    })
  }
}
</script>

<style>
</style>
