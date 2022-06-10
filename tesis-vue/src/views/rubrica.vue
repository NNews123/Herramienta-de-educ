<template>
<div>
          <v-layout>
              <v-flex class="fondog m0 p0" white--text>
                <h1 class="display1"><v-icon large class="material-icons-outlined">assignment_turned_in</v-icon>Rúbrica</h1>
                <v-btn dark color="#BDBDBD" flat depressed elevation="2">
                  <span large class="material-icons">west</span>
                  <h3>Regresar</h3>
                </v-btn>
              </v-flex>
          </v-layout>
 
  <v-container >

    
      <template>

        <v-card>
          <v-toolbar
            flat
            color="orange lighten-1"
            dark
          >
            <v-toolbar-title>Nueva rúbrica</v-toolbar-title>
          </v-toolbar>

          <v-card-text>
            <v-text-field
              filled
              label="Nombre de la actividad"
              value=""
            ></v-text-field>

           <v-textarea
                label="Descripción"
                auto-grow
                filled
                rows="1"
                row-height="15"
            ></v-textarea>

            <v-divider class="my-2"></v-divider>

            <!-- Aquí comienza la tabla -->
            <v-item-group multiple>
                    <v-layout>
                      <v-row justify="center">
                        <v-col
                          cols="12"
                          sm="8">
                                  <v-simple-table>
                                      <thead class="orange lighten-1">
                                        <tr>
                                          <th class="text-center">
                                            <h2>Criterios</h2>
                                          </th>
                                          <th class="text-center">
                                            <h2>Exelente</h2>
                                          </th>
                                          <th class="text-center">
                                            <h2>Muy buena</h2>
                                          </th>
                                          <th class="text-center">
                                            <h2>Bueno</h2>
                                          </th>
                                          <th class="text-center">
                                            <h2>Regular</h2>
                                          </th>
                                          <!-- <th class="text-left">
                                            <h2>¿Cumple?</h2>
                                          </th> -->
                                        </tr>
                                      </thead>
                                      <tbody>
                                        <tr>
                                          <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>

                                          <!-- esta parte de codigo agrega los botones para seleccionar los criterios de evaluacion y se repite 2 veces mas abajo -->

                                         <!--  <td>
                                              <v-radio-group
                                                    v-model="column"
                                                    column
                                                  >
                                                    <v-radio
                                                      label="Si"
                                                      value="radio-1"
                                                    ></v-radio>
                                                    <v-radio
                                                      label="No"
                                                      value="radio-2"
                                                    ></v-radio>
                                              </v-radio-group>
                                          </td> -->
                                        </tr>
                                        <tr>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                         <!--  <td>
                                              <v-radio-group
                                                    v-model="column"
                                                    column
                                                  >
                                                    <v-radio
                                                      label="Si"
                                                      value="radio-1"
                                                    ></v-radio>
                                                    <v-radio
                                                      label="No"
                                                      value="radio-2"
                                                    ></v-radio>
                                              </v-radio-group>
                                          </td> -->
                                        </tr>
                                        <tr>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                           <td>
                                              <v-textarea
                                                label="agregar criterio"
                                                auto-grow
                                                rows="1"
                                                row-height="15"
                                              ></v-textarea>
                                          </td>
                                          <!-- <td>
                                           <v-radio-group
                                                    v-model="column"
                                                    column
                                                  >
                                                    <v-radio
                                                      label="   Si"
                                                      value="radio-1"
                                                    ></v-radio>
                                                    <v-radio
                                                      label="No"
                                                      value="radio-2"
                                                    ></v-radio>
                                              </v-radio-group>
                                          </td> -->
                                        </tr>
                                      </tbody>
                                  </v-simple-table>
                          </v-col>
                        </v-row>
                    </v-layout>
            </v-item-group>
            <!-- aquí termina la tabla -->
          </v-card-text>

          <!-- Botones de agregar y quitar campos en la lista de cotejo -->

          <v-card-actions>
          <v-btn
              class="mx-2"
              fab
              dark
              small
              color="red"
              >
                <v-icon  large center>
                    remove
                </v-icon>
          </v-btn>
            <v-spacer></v-spacer> 
            <v-btn
              class="mx-2"
              fab
              dark
              small
              color="green"
              left
              >
                <v-icon dark large center>
                      add
                </v-icon>
            </v-btn>
          </v-card-actions>
          
        </v-card>

        <!-- Botones de guardar los criterios de la lista de cotejo -->
        <br>
        <v-layout justify-center>
            <v-btn
                  depressed
                  color="primary"
                >
              Guardar
            </v-btn>
            <v-btn
                  depressed
                  color="secondary"
                >
              Salir
            </v-btn>
        </v-layout>     

      </template>

  </v-container>

  <!-- Aqui se realiza el footer -->

          <v-footer
            v-bind="localAttrs"
            fixed tile absolute
            padless
          >
            <v-card
              flat
              tile
              lg
              width="100%"
              class="light-green darken-3 white--text text-center"
            >
              <v-card-text class="white--text">
                {{ new Date().getFullYear() }} — <strong>Derechos reservados para el autor</strong>
              </v-card-text>
            </v-card>
          </v-footer>
  
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

