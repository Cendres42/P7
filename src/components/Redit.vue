<template>
<div id="msgaccueil">
  <h1> {{messagebjr}} </h1>
<div id="signup">
  <h2> Insciption au réseau social de Groupomania</h2>
  <p> Pour vous inscrire, veuillez remplir toutes les rubriques de ce formulaire, merci! </p>
  <form  novalidate name="client" id="form_1">
    <div class="form-group">
      <label class="label" for="nom">	Nom	</label>
      <input type="text" name="nom" id="nom" title="nom" class="form-control" pattern="[A-Za-z]{3,20}" required/>
      <span id="missNom"></span>
    </div>
    <div class="form-group">
      <label class="label" for="prenom">	Prénom	</label>
      <input type="text" name="prenom" id="prenom" title="prénom" class="form-control" pattern="[A-Za-z]{3,20}" required />
      <span id="missPrenom"></span>
    </div>
    <div class="form-group">
      <label class="label" for="email">	Adresse email	</label>
      <input type="email" name="email" id="email" title= "adresse mail" class="form-control" required />
      <span id="missEmail"></span>
    </div>
    <div class="form-group">
      <label class="label" for="mdp">	Mot de passe	</label>
      <input type="password" name= "mdp" id="mdp" title=" mdp" class="form-control" minlength="6" required  />
      <span id="missMdp"></span>
    </div>
    <button id="envoi" class="button" type="submit">Valider l'inscription </button>
   </form>
 </div>

<div id="login">
  <h2> Connexion au réseau social de Groupomania</h2>
  <p> Entrez le mail et le mot de passe utilisés pour vous inscrire</p>
  <div class="form-group">
    <label class="label" for="email">	Adresse email	</label>
    <input type="email" name="email" id="email" title= "adresse mail" class="form-control" required />
    <span id="missEmail"></span>
  </div>
  <div class="form-group">
    <label class="label" for="mdp">	Mot de passe	</label>
    <input type="password" name= "mdp" id="mdp" title=" mdp" class="form-control" minlength="6" required  />
    <span id="missMdp"></span>
  </div>
  <button id="envoi" class="button" type="submit"> Connexion </button>
</div>
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
.logo, #msgaccueil {
  text-align: center;
}

button, h2{
  color:red;
  margin-bottom:0.5em;
}
#msgaccueil{
  background-image: url("../assets/icon.png");
  background-repeat: no-repeat;
  background-position: center;
  height:50em;
  text-align: center;
  padding-top:6em;
}

.form-control {
  margin-bottom:1em;
  margin-left:2em;
}
label
{
    display:block;
    width:100px; /* Attention : prenez une largeur suffisamment grande */
    float:left;

}
.form-group{
  width:20em;
  margin-left: 30em;
}

</style>
