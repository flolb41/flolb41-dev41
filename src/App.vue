<template>
  <div id="app">
    <div class="header">
      <div class="heading">
        <h1>Florian Le Blanc</h1>
        <div id="nav">
          <router-link to="/">Accueil</router-link> |
          <router-link to="/about">Qui suis-je ?</router-link>
        </div>
      </div>
      <router-view />
    </div>
    <Footer />
  </div>
</template>
<script>
import Footer from './components/Footer.vue';
export default {
  name: "App",
  components: { Footer },
};
</script>
<style>
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: rgb(238, 238, 255);
  background: linear-gradient(to top, rgba(255, 255, 255, 0) -70%, rgb(0, 0, 124)),
    url("./assets/code-ex.jpg");
  background-repeat: repeat;
  min-height: 100%;
  margin: 0;
}
.header {
  display: flex;
  flex-direction: column;
}
.heading {
  padding: 1%;
  background-color: black;
  display: flex;
  justify-content: space-between;
}
h1 {
  color: white;
  margin: auto 10%;
  font-family: 'Oregano', cursive;
  font-size: 2.8em;
}
#nav {
  margin: auto 10%;
}
#nav a {
  color: grey;  
  text-decoration: none;

}
#nav a.router-link-exact-active {
  color: white;
}
footer {
  bottom: 0;
}
@media screen and (max-width: 700px) {
  h1 {
    margin: 2%;
    width: 50%;
    font-size: 150%;
  }
  #nav {
    margin: 2%;
    font-size: 90%;
  }
}
</style>
