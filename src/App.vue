<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/contact">Contact</router-link>
    </div>

    <!-- Dans ton App.vue tu ne mets seulement la barre de navigation et
    ce routerview qui se charge d'afficher ce qui est passé dans l'URL,
    si l'URL se fini par /contact. Le routerview se charge d'afficher
    la page Contact.vue dans le dossier view.
    Pourquoi ?
    Dans le dossier router il y a un fichier qui s'appelle index.js.
    Dans celui-ci on déclare toutes les routes possible (donc les urls)
    On peut voir la page Home, About et Contact. Il faut les ajouter
    a partir d'ici (ne pas oublier de les importer tout en haut du fichier)
    Je t'ai également mis un petit bonus dans le fichier router/index.js
    qui pourra t'être utile, il redirige automatiquement sur la page d'accueil
    si l'URL n'existe pas.
    J'espère avoir résolu ton problème, si tu as besoin, tu peux aller voir
    le code de mes autres projets, cela pourrait t'être utile.
    Bonne journée-->
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
