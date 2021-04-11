<template>
  <footer class="text-center text-lg-start">
    <div class="container p-4">
          <ul class="list-unstyled mb-0">
            <li>
              <a href="https://github.com/flolb41"
                ><i class="fab fa-github"></i><span>Github.com</span></a
              >
            </li>
            <li>
              <a href="https://www.linkedin.com/in/florian-le-blanc-0291b11ab/"
                ><i class="fab fa-linkedin"></i><span> Linkedin.com</span></a
              >
            </li>
            <li>
              <a href="https://www.malt.fr/profile/florianleblanc2"
                ><img src="@/assets/malt-logo.jpg" alt="logo Malt" /><span> Malt.fr</span></a
              >
            </li>
            <li>
              <a href="https://my.indeed.com/p/florianl-uiucx5s"
                ><img src="@/assets/indeed.png" alt="logo Indeed" /><span>
                Indeed.com</span></a
              >
            </li>
            <li>
              <a href="https://www.freelancer.com/u/flolb41"
                ><img src="@/assets/freelancer.png" alt="logo Freelancer" /><span>
                Freelancer.com</span></a
              >
            </li>
            <li>
              <a href="https://www.codeur.com/-florianlv5mp"
                ><img src="@/assets/codeur.jpeg" alt="logo Codeur" /><span>
                Codeur.fr</span></a
              >
            </li>
          </ul>
        </div>
  </footer>
</template>
<script>
export default {};
</script>
<style >
footer {
  background-color: black;
  font-family: "Trebuchet MS", "Lucida Sans Unicode", "Lucida Grande",
    "Lucida Sans", Arial, sans-serif;
  font-size: 0.5em;
  position: fixed;
  bottom: 0;
  width: 100%;
}
footer i {
  font-size: 3em;
  color: blue;
  margin-right: 10px;
}
footer a {
  color: rgb(166, 166, 255);
  text-decoration: none;
  font-size: 1.5em;
}
footer span {
  display: block;
  width: 100px;
}
footer img {
  height: 30px;
  margin-right: 10px;
}
footer .row {
  justify-content: space-around;
  width: 100%;
  margin: 0 10px;
}
footer .group {
  padding: 0;
}
footer .list-unstyled {
  text-align: left;
  list-style: none;
  display: flex;
  justify-content: space-around;
}
footer li {
  width: 50%;
  margin: auto 3%;
}
@media screen and (max-width: 800px) {
  footer .group {
    margin: 0 auto;
  }
  footer li {
    margin: auto 5px;
  }
  footer span {
    display: none;
  }
  footer ul {
    margin-left: 3%;
  }
}
</style>