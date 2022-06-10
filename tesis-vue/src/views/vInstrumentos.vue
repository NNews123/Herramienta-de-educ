<template>
  <div>
    
      <template>
        <v-card height="400px">
              <v-footer
                v-bind="localAttrs"
                fixed tile absolute
              >
                <v-card
                  flat
                  tile
                  lg
                  width="110%"
                  class="light-green darken-3 white--text text-center"
                >
                  <v-card-text>
                    <v-btn      
                      v-for="icon in icons"
                      :key="icon"
                      class="mx-4"
                      icon
                    >
                      <v-icon size="24px">
                        {{ icon }}
                      </v-icon>
                    </v-btn>
                  </v-card-text>

                  <v-divider></v-divider>

                  <v-card-text class="white--text">
                    {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
                  </v-card-text>
                </v-card>
              </v-footer>

        </v-card>
      </template>
  </div>
</template>


<script>
  
  export default {
    
    data: () => ({

      items: ['rubrica mapa conceptual','lista de cotejo mapa conceptual','lista de cotejo practica 1', 'rubrica para practica de laboratorio de redes'],
      items2: ['1','2','3','4','5','6','7','8','9','10','11','12','13','14','15'],
      icons: ['mdi-facebook','mdi-twitter','mdi-linkedin','mdi-instagram',],
      dialogban: false,
      ex7: 'red',
      ex8: 'primary',
      value: null,

    }),

    }

</script>