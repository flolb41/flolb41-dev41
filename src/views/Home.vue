<template>
  <div class="home">
    <div class="slogan">
      <h2>Misez sur le Web</h2>
      <p>
        Professionnel, Association, Particulier, Artiste, Créateur, Designer<br />
        N'attendez plus, l'ère de la digitalisation a sonné.
      </p>
      <p>Obtenez plus de visibilité et soyez accessible sur le net.</p>
    </div>
    <div class="service">
      <h2>Je suis là pour vous aider</h2>
      <p>Du grand au petit projet, du grand au petit budget,<br>je peux vous créer:</p>
      <ul>
        <li>un CV original et accessible sur le net</li>
        <li>une landing-page</li>
        <li>un site vitrine</li>
        <li>un blog</li>
        <li>une boutique</li>
        <li>un forum, boite à idées pour vos salariés</li>
        <li>Et bien d'autres encore...</li>  
      </ul>
      <router-link to='/Contact' class="btn btn-primary">Contactez moi !!</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
<style>
.home {
  display: flex;
  flex-direction: column;
  margin: 50px 0 100px;
  height: auto;
}
h2 {
  text-decoration: underline;
}
.home p {
  margin: 0 auto;
  font-size: 1.2em;
}
.slogan, .service {
  font-family: "Oregano", cursive;
  font-size: 1.5em;
  word-spacing: 5px;
  border: 3px solid white;
  width: 70%;
  margin: 1% auto;
  padding: 0 1%;
}
.slogan {
  border-radius: 50px 150px 10px 0px;
}
.service {
  border-radius: 0px 5px 50px 150px;
}
.service ul {
  width: 80%;
  margin: 2% auto;
}
.service ul li {
  text-align: left;
}
.service a {
  display: block;
  width: 200px;
  margin: 1% auto;
  padding: 10px;
  font-size: 1em;
  background-color: lime;
  color: black;
  border-radius: 10px;
  text-decoration: none;
}
.service a:hover {
  transition: ease-in-out;
  transition-duration: 0.5s;
  background-color: green;
}
@media screen and (max-width: 700px) {
  .home {
    margin: 10px 0 100px 0;
  }
  .service ul {
    width: 90%;
    margin: 2%;
  }
  .slogan, .service {
    font-size: 100%;
    width: 97%;  
    padding: 10px;
  }
  .slogan {
  border-radius: 25px 100px 5px 5px;
}
  .service {
    border-radius: 5px 5px 25px 100px;
    margin: 10px auto;
  }
  .service a {
    width: 150px;
  }
}
</style>