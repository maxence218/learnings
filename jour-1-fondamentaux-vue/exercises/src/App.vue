<script setup>
  import { capitalize } from 'vue';
  const name = "maxence"
  const age = 29
  const ville = "Tourcoing"

  const personne = {
    nom: "maxence",
    age: 29,
    poste: "developpeur Front-End",
    email: "maxencemaho@gmail.com",
    competence: ["Vue.js", "React.js", "TypeScript"],
    photo_url: "https://media.licdn.com/dms/image/v2/D4E35AQG5rqH2lSc03w/profile-framedphoto-shrink_200_200/B4EZshQGmaIQAY-/0/1765789428390?e=1767610800&v=beta&t=WUt-LZceslVN2JtIOrLqoqaI33reKkJ7xKYTf0btFgY",
    linkedin_url: "https://www.linkedin.com/in/maxence-maho-295537294/",
    github_url: "https://github.com/maxence218",
  }
</script>

<template>
  <main>
    <!-- <p>je m'appelle {{ name }} et j'ai {{ age }}, j'habite a {{ ville }}</p>
    <p>Dans 10ans  j'aurais {{ age + 10 }}</p>
    <p>Mon nom en majuscule {{ name.toUpperCase() }}</p> -->
<div class="container">
  <div class="card">
    <h1>{{ capitalize(personne.nom) }}</h1>
    <h2>Age : {{ personne.age }}</h2>
    <h2>Competence : {{ personne.competence.length }} </h2>
    <h3> {{ personne.competence.join(', ') }}</h3>
    <h2>Email : {{ personne.email }}</h2>
    <img :src="personne.photo_url" alt="Ma photo">
    <p>Folow me on : <a :href="personne.linkedin_url">Mon Linkedin</a> - <a :href="personne.github_url"> Mon Github</a> </p>
  </div>
</div>
  </main>
</template>

<style scoped>
main {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.card {
  max-width: 400px;
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  text-align: center;
  background: white;
}

img {
  width: 150px;
  border-radius: 50%;
  margin: 1rem 0;
}

a {
  color: #42b883;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}
</style>
