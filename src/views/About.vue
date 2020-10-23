<!-- Template-->
<template>
  <div class="container">
    <h1 class="tituloAbout">About</h1>
    <img src="assets/img/rick-logo.png" class="imgRym" />
    <div class="textoAbout">
      <p>
        Rick y Morty (en inglés: Rick and Morty) es una serie de televisión
        estadounidense de animación para adultos creada por Justin Roiland y Dan
        Harmon en 2013 para Adult Swim.<br />
        La serie sigue las desventuras de un científico, Rick, y su fácilmente
        influenciable nieto, Morty, quienes pasan el tiempo entre la vida
        doméstica y los viajes espaciales, temporales e intergalácticos. <br />
        Roiland es el encargado de darle voz a los dos personajes principales, y
        la serie también incluye las voces de Chris Parnell, Spencer Grammer y
        Sarah Chalke.
      </p>

      <p>
        Los orígenes de la serie pueden encontrarse en un cortometraje
        rudimentario animado por Roiland para el festival de cine Channel 101
        llamado Doc and Mharti, una parodia de los principales protagonistas de
        Back to the Future. Cuando la cadena NBC despidió a Harmon en 2013 por
        discusiones entre él y los ejecutivos de la serie que había creado,
        Community, él y Roiland desarrollaron una serie basada en los personajes
        ya creados por Roiland.1​
      </p>
    </div>
  </div>
</template>

<!-- Script -->
<script>
export default {
  name: "About",
};
</script>

<!-- Style -->
<style scoped>
.tituloAbout {
  margin-top: 20px;
  text-align: center;
  font-family: "Grandstander", sans-serif;
  color: rgb(59, 59, 59);
}
.imgRym {
  max-width: 60%;
  display: block;
  margin: auto;
  padding-bottom: 50px;
}
.textoAbout {
  padding-bottom: 50px;
  color: rgba(68, 68, 68, 0.658);
  font-weight: 500;
  font-size: 18px;
}
</style>
