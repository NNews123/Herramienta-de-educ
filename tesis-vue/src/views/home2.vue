<template>
<div>
          <v-layout>
              <v-flex class="fondog m0 p0" white--text>
                <h1 class="display1"><v-icon class="material-icons">list</v-icon>Asignar instrumento</h1>
                <v-btn dark color="#BDBDBD" flat depressed elevation="2">
                  <span large class="material-icons">west</span>
                  <h3>Regresar</h3>
                </v-btn>
              </v-flex>
          </v-layout>
  <v-container >

    <v-layout>
      <v-btn color="blue" large dark @click="dialogban= true"> <v-icon>add</v-icon> Crear nuevo intrumento</v-btn>
    </v-layout>
     <v-layout wrap>
        <v-expansion-panels>
          <v-expansion-panel>
            <v-expansion-panel-header disable-icon-rotate>
              Actividad 1
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>
            <v-expansion-panel-content>
              instrumento
              <v-autocomplete  rounded solo auto-select-first chips clearable
               v-model="values"
               :items="items"
              ></v-autocomplete>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header disable-icon-rotate>
              Actividad 2
              <template v-slot:actions>
                <v-icon color="teal">done</v-icon>
              </template>
            </v-expansion-panel-header>
            <v-expansion-panel-content>
              instrumento
                    <v-autocomplete  rounded solo auto-select-first clearable 
                    v-model="values"
                    :items="items"
                    ></v-autocomplete>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header disable-icon-rotate>
              Actividad 3
              <template v-slot:actions>
               <v-icon color="red" class="material-icons">info</v-icon>
              </template>
            </v-expansion-panel-header>
            <v-expansion-panel-content>
              instrumento
              <v-autocomplete  rounded solo auto-select-first chips clearable
               v-model="values"
               :items="items"
              ></v-autocomplete>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
              <v-expansion-panel-header disable-icon-rotate>
                Actividad 4
                <template v-slot:actions>
                <v-icon color="red" class="material-icons">info</v-icon>
                </template>
              </v-expansion-panel-header>
              <v-expansion-panel-content>
                instrumento
                <v-autocomplete  rounded solo auto-select-first chips clearable
                v-model="values"
                :items="items"
                ></v-autocomplete>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header disable-icon-rotate>
              Actividad 5
              <template v-slot:actions>
                <v-icon color="teal">done</v-icon>
              </template>
            </v-expansion-panel-header>
            <v-expansion-panel-content>
              instrumento
                    <v-autocomplete  rounded solo auto-select-first clearable 
                    v-model="values"
                    :items="items"
                    ></v-autocomplete>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header disable-icon-rotate>
              Actividad 6
              <template v-slot:actions>
                <v-icon color="primary">hourglass_disabled</v-icon>
              </template>
            </v-expansion-panel-header>
            <v-expansion-panel-content>
              instrumento
              <v-autocomplete  rounded solo auto-select-first chips clearable
               v-model="values"
               :items="items"
              ></v-autocomplete>
            </v-expansion-panel-content>
          </v-expansion-panel>
          

       </v-expansion-panels>
     </v-layout>
    
    <v-layout>
     
     <v-dialog v-model="dialogban" width="600" persistent class="text-center">
       <v-card>
         <v-card-title><h3>¿Qué deseas agregar?</h3></v-card-title>
         <v-card-text>
            <v-radio-group v-model="ex7" column>
                  
                  <v-radio
                      label="Lista de cotejo"
                      color="indigo"
                      value="Lista de cotejo"
                  ></v-radio>     
                  <v-radio
                      label="Rúbrica"
                      color="orange"
                      value="Rúbrica"
                  ></v-radio>  
            </v-radio-group>
            <v-select
                    :items="items2"
                    :menu-props="{ top: true, offsetY: true }"
                    label="Criterios"
            ></v-select>
         </v-card-text>
         <v-divider></v-divider>
         <v-card-action>
           <v-btn dark @click="dialogban=false">Cerrar</v-btn>
         </v-card-action>
         <v-card-action>
           <v-btn dark color="blue" @click="dialogban=false">Guardar</v-btn>
         </v-card-action>
       </v-card>
     </v-dialog>



    </v-layout>

    
  </v-container>
 
<template>
  <v-card height="500px">
        <v-footer
          v-bind="localAttrs"
          fixed tile absolute
          padless
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
                dark
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


  <!-- <template>
    <v-footer fixed tile absolute  :padless="padless">
      <v-card  lg flat tile class="light-green darken-3 white--text text-center">

        <v-card-text class="white--text">Derechos de autor de la Universidad de Colima Derechos de autor de la Universidad de Colima Derechos de autor de la Universidad de Colima Derechos de autor de la Universidad de Colima Derechos de autor de la Universidad de Colima Derechos de autor de la Universidad de Colima</v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-card-text>
      </v-card>
  </v-footer>
  
  </template> -->
  
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
