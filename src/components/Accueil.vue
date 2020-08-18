<template>
  <div id="msgaccueil">
    <h1> Bienvenue sur le réseau social Groupomania </h1>
    <button> Envie d'échanger avec vos collègues autour de contenus multimédias?<br>
         9GAG est fait pour vous!</button>
    <button> Envie de partager des articles avec vos collègues?<br>
              Redit est fait pour vous!</button>
  </div>
</template>

<script>
export default {
  name: 'Accueil',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
