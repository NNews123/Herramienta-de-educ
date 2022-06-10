<template>
  <v-app>
    <v-app-bar
      app
      color="#558B2F"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-4"
          contain
          src="http://educ.ddns.net:88/listadocursos/assets/img/logos/logo_educ_heade_blanco.png"
          transition="scale-transition"
          width="110"
        />
      </div>

      <v-spacer></v-spacer>

<!-- Boton direcciona a pagina de los instrumentos -->
      <v-btn
        href="./views/rubrica.vue"
        target="_blank"
        text
      >
        
        <span class="mr-2">instrumentos</span>
        <v-icon color="white" class="material-icons">text_snippet</v-icon>
      </v-btn>
    </v-app-bar>
    
 <!--  se agrego el boton de regresar en la barra princial -->
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

