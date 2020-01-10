<template>
  <div id='app'>
    <div class='container d-flex flex-column align-items-center'>
      <h3>Flash Cards!</h3>
      <FlashCard sideA='Sorry' sideB='Signomi' />
    </div>
  </div>
</template>

<script>
import FlashCard from './components/FlashCard.vue'

export default {
  name: 'app',
  components: {
    FlashCard
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
