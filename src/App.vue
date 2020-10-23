<!-- Template -->
<template>
<div>
  <v-app>
    <v-toolbar dense  height="80px" dark >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Rick & Morty</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn ><router-link :to="{ name: 'Inicio' }" class="linkNav" style="text-decoration:none" >Inicio</router-link></v-btn>
      <v-btn ><router-link :to="{ name: 'Buscar' }" class="linkNav" style="text-decoration:none" >Buscar</router-link></v-btn>
      <v-btn ><router-link :to="{ name: 'About' }" class="linkNav" style="text-decoration:none" >About</router-link></v-btn>
    </v-toolbar>
    <router-view class="contenidoPagina"></router-view>
 
  </v-app>
  </div>
</template>

<!-- Script -->
<script>
export default {
  name: "App",
};
</script>

<!-- Style -->
<style scoped>
.linkNav {
  color: white;
}

</style>