<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
   
    <SlotComponent>
      <template>
       <img src="./assets/pic/04.png" />
      </template>
    </SlotComponent>
    <Count/>
  </div>
</template>

<script>
import SlotComponent from './components/SlotComponent.vue'
import Count from './components/Count.vue'

export default {
  name: 'App',
  components: {
    SlotComponent,
    Count
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
