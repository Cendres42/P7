<template>
  <div id="app">
    <img src="./assets/logo.jpg" alt=logo Groupomania/>
    <Accueil msg=""/>
    <Redit msg=""/>
  </div>
</template>

<script>
import Accueil from './components/Accueil.vue'
import Redit from './components/Redit.vue'

export default {
  name: 'App',
  components: {
    Accueil,
    Redit,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
