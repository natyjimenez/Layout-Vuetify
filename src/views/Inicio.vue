<!-- Template -->
<template>
  <div class="home">
    <v-main>
      <h1 class="titulo">Personajes Rick & Morty</h1>
      <v-container>
        <v-row :justify="start">
          <v-col md="4" v-for="(personaje, i) in personajes" :key="i">
            <v-card class="mx-auto" max-width="344">
              <v-img :src="personaje.imagen" height="180px"></v-img>

              <v-card-title class="tituloCard">
                {{ personaje.nombre }}
              </v-card-title>

              <v-card-actions>
                <v-spacer></v-spacer>

                <v-btn icon @click="personaje.show = !personaje.show">
                  <v-icon>
                    {{ personaje.show ? "mdi-chevron-up" : "mdi-chevron-down" }}
                  </v-icon>
                </v-btn>
              </v-card-actions>

              <v-expand-transition>
                <div v-show="personaje.show">
                  <v-divider></v-divider>

                  <v-card-text class="infoCard">
                    Estado: {{ personaje.estado }}<br />
                    Especie: {{ personaje.especie }}<br />
                    Género: {{ personaje.genero }}
                  </v-card-text>
                </div>
              </v-expand-transition>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </div>
</template>

<!-- Script --> 
<script>
export default {
  name: "Inicio",
  data: () => ({
    personajes: [
      {
        id: 1,
        nombre: "Morty",
        imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        show: false,
        estado: "Vivo",
        especie: "Humano",
        genero: "Masculino",
      },
      {
        id: 2,
        nombre: "Rick",
        imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        show: false,
        estado: "Vivo",
        especie: "Humano",
        genero: "Masculino",
      },
      {
        id: 3,
        nombre: "Summer",
        imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        show: false,
        estado: "Vivo",
        especie: "Humano",
        genero: "Femenino",
      },
      {
        id: 4,
        nombre: "Beth",
        imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        show: false,
        estado: "Vivo",
        especie: "Humano",
        genero: "Femenino",
      },
      {
        id: 5,
        nombre: "Jerry",
        imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        show: false,
        estado: "Vivo",
        especie: "Humano",
        genero: "Masculino",
      },
    ],
  }),
};
</script>

<!-- Style -->
<style scoped>
.titulo {
  text-align: center;
  margin-top: 30px;
  margin-bottom: 20px;
  font-family: "Grandstander", sans-serif;
  color: rgb(59, 59, 59);
}
.tituloCard {
  color: rgb(18, 133, 8);
  font-weight: 700;
}
.infoCard {
  color: rgba(68, 68, 68, 0.658);
  font-weight: 500;
  font-size: 18px;
}
</style>
