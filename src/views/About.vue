<template>
  <div class="about">
    <section class="presentation">
      <img alt="Vue logo" src="../assets/logo.png" />
      <h2 class="moi">Un peu plus sur moi...</h2>
      <p>
        Alors que je n'ai que 6 ans, mes parents sautent le pas et découvrent
        l'informatique en 1990 en acquérant le premier pc familial. Un Amstrad
        PC3086. Je ferai mes premières armes dessus, devenant très vite "accro".
        Je passerai ainsi plusieurs années de ma jeunesse à découvrir,
        l'overclocking, le watercooling entre autres... dans une chambre
        transformée en atelier de geek. Après une scolarité ou mes profs disent
        toujours "Pourrait tutoyer les sommet si il s'en donnait la peine !", je
        parviens jusqu'au bac.<br /><br />
        Après avoir choisi STI électronique, et avoir obtenu le diplôme en 2003,
        j'intègre l'école de Maistrance à Brest, école de sous-officier de la
        Marine Nationale. Où je me rends vite compte que je manque d'air...
        J'enchaine ensuite les petits boulots, qui, avec le recul auront été une
        bonne "école".<br /><br />
        En 2007, j'entre dans le transport de fond complètement par hasard,
        suite à une annonce ANPE (et oui, à l'époque Pole Emploi n'existe pas
        encore...) Je me fais un nom dans le milieu, en travaillant même à tour
        de rôle pour les deux plus gros concurrents. J'apprécie le métier, mais
        au bout de 13 ans, une maladie professionnelle me touche et mets fin à
        cette aventure.<br /><br />
        En arrêt depuis Aout 2019, et sachant mon avenir de plus en plus sombre
        dans ce métier, j'en profite pour faire le point moi-même. Très vite, je
        me rends compte que ce licenciement sera un mal pour un bien. Car, lors
        d'une discussion avec mon père, il me fait part d'un reportage qu'il a
        vu sur les métiers qui recrutent. C'est lui qui me mets la puce à
        l'oreille. J'en profite donc pour mettre tout ce temps en arrêt de
        travail pour apprendre et me former. Je suis officiellement licencié en
        avril 2020, Ayant déjà quelques notions de code, je décide
        d'officialiser mes connaissances avec une formation reconnue bac + 2
        chez OpenClassrooms. Formation que je valide fin mars 2021.
      </p>
    </section>
    <section class="formation">
      <div class="timeline-container">
        <div class="timeline-block timeline-block-right">
          <div class="marker"></div>
          <div class="timeline-content">
            <h3>2021 - Développeur web - bac +2</h3>
            <span>OpenClassrooms</span>
            <p>Formation comportant plusieurs projets de mise en situation. Les projets se suivent avec une difficulté croissante, permettant de se familiariser avec les langages tels que HTML5 / CSS3 au début, puis Javascript, enfin un framework.
              Cette formation traite du front-end ainsi que du back-end.
            </p>
          </div>
        </div>
        <div class="timeline-block timeline-block-left">
          <div class="marker"></div>
          <div class="timeline-content">
            <h3>2003 - Baccalauréat STI électronique</h3>
            <span>Lycée Augustin Thierry</span>
            <p>Diplôme orienté en éléctronique, apprenant les bases ( loi d'ohm, langage binaire ou hexadecimal ) </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  name: "About",
  data: () => {
    return {
      diplomes: [
        {
          id: 1,
          name: "Développeur web",
          grade: "Bac +2",
          ecole: "OpenClassrooms",
          lieu: "Paris",
          annee: "2021",
        },
        {
          id: 2,
          name: "Baccalauréat STI option électronique",
          grade: "Bac",
          ecole: "Lycée Augustin Thierry",
          lieu: "Blois",
          annee: "2003",
        },
      ],
      emplois: [
        {
          id: 1,
          societe: "Loomis",
          poste: "Convoyeur de fonds - chef de bord",
          epoque: "11-2013 à 04-2020",
        },
        {
          id: 2,
          societe: "Brink's",
          poste: "Convoyeur de fonds - chef de bord",
          epoque: "04-2012 à 11-2013",
        },
        {
          id: 3,
          societe: "Loomis",
          poste: "Convoyeur de fonds - chef de bord",
          epoque: "05-2007 à 04-2012",
        },
      ],
    };
  },
};
</script>
<style>
.about {
  display: flex;
  flex-direction: column;
  margin-bottom: 100px;
}
.about img {
  min-width: 130px;
  width: 15%;
  border-radius: 10px;
  float: left;
  margin: 50px 20px 20px 50px;
}
.about h2 {
  margin: 30px auto;
}
.about p {
  font-size: 1em;
  text-align: justify;
  margin: auto 50px;
}
.about .formation {
  margin: auto;
  text-align: left;
}
.about .diplomes {
  margin: 50px auto;
}
.about h4 {
  text-decoration: underline;
}
.about * {
   -webkit-box-sizing: border-box;
   -moz-box-sizing: border-box;
   box-sizing: border-box;
   outline: none;
}
.about body {
   margin: 0;
   font-family: 'Roboto', sans-serif;
   background: #F1F2F6;
}
.formation .timeline-container {
  width: 90%;
  padding: 50px 0;
  margin: 20px auto;
  position: relative;
  overflow: hidden;
  z-index: 0;
}
.formation .timeline-container:before {
  /*This is the line down the middle*/
  content: "";
  position: absolute;
  top: 0;
  left: 50%;
  margin-left: -1px;
  width: 2px;
  height: 80%;
  background: #ccd1d9;
  z-index: 1;
}
.formation .timeline-block {
  width: -webkit-calc(50% + 8px);
  width: -moz-calc(50% + 8px);
  width: calc(50% + 8px);
  display: -webkit-box;
  display: -webkit-flex;
  display: -moz-box;
  display: flex;
  -webkit-box-pack: justify;
  -webkit-justify-content: space-between;
  -moz-box-pack: justify;
  justify-content: space-between;
  clear: both;
}
.formation .timeline-block-right {
  float: right;
}
.formation .timeline-block-left {
  float: left;
  direction: rtl;
}
.formation .marker {
  width: 16px;
  height: 16px;
  border-radius: 50%;
  border: 2px solid #f5f7fa;
  background: #4dd0e1;
  margin-top: 10px;
  z-index: 9999;
}
.formation .timeline-content {
  width: 100%;
  padding: 0 15px;
  color: rgb(255, 255, 255);
}
.formation .timeline-content h3 {
  margin-top: 5px;
  margin-bottom: 5px;
  font-size: 25px;
  font-weight: 500;
}
.formation .timeline-content span {
  font-size: 15px;
  color: #ffffff;
}
.formation .timeline-content p {
  font-size: 16px;
  line-height: 1.5em;
  word-spacing: 1px;
  color: rgb(255, 255, 255);
}
@media screen and (max-width: 768px) {
  .about {
    margin-bottom: 100px;
  }
  .about .formation {
    margin: 10px;
  }
  .formation .timeline-container:before {
    left: 8px;
    width: 2px;
  }
  .formation .timeline-block {
    width: 100%;
    margin-bottom: 10px;
  }
  .formation .timeline-block-right {
    float: none;
  }
  .formation .timeline-block-left {
    float: none;
    direction: ltr;
  }
  .formation .timeline-content h3 {
    font-size: 100%;
  }
  .formation .timeline-content p {
    font-size: 90%;
  }
}
</style>