<template>
  <div class="contact">
<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdUIB57DyAOfvgoFvL6OIUAsb5cKcoU7X2B24h94tKmuDVGdg/viewform?embedded=true" width="640" height="750" frameborder="0" marginheight="0" marginwidth="0">Chargement…</iframe>
  </div>
</template>
<script>

export default {
    name: 'Contact',
};
</script>
<style scoped>
.contact {
    display: flex;
    flex-direction: column;
    height: 80vh;
    margin: 2% 0;
}
h2 {
    font-family: 'Oregano', cursive;
}
form {
    width: 60%;
    margin: 10% auto;
}
.col-4 {
    margin: auto;
}
iframe {
    width: 50%;
    margin: auto;
}
@media screen and (max-width: 700px) {
    iframe {
        width: 80%;
    }
}
</style>