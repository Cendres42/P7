<template>
  <div id="app">
    <img src="./assets/logo.jpg" alt=logo Groupomania/>
    <div id="nav">
      <router-link to="/">Accueil</router-link> |
      <router-link to="/9GAG">9GAG</router-link> |
      <router-link to="/Redit">Redit</router-link>
    </div>
    <router-view></router-view>
  </div>
</template>


<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
