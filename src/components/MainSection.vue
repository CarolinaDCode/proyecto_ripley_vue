<template>
  <div class="px-10">
    <v-container>
      <div class="my-5 d-flex justify-center">
        <img src="../assets/cintillo_middle_desk.webp" max-width="1100" >
      </div>

      <v-row class="d-flex">
        <v-col
            cols="7"
        >
          <v-img
              width="880"
              height="229"
              src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/BANNER_BLANDOS/1.jpg?v1"
          />
        </v-col>
        <v-col
            cols="5"
        >
          <v-img
              width="880"
              height="229"
              src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/BANNER_BLANDOS/2m.jpg"
          />
        </v-col>
      </v-row>
      <h1 class=" d-flex justify-center mt-5 card_title " >
        <strong>para mascotas, </strong><span class="font-weight-light">lo tenemos todo</span>
      </h1>
      <v-row>
        <v-col
            cols="6">
          <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/banner_desk.webp"/>

        </v-col>
        <v-col
            cols="6"
        >
          <v-carousel
              v-model="model"
              cycle
              hide-delimiter-background
              show-arrows
          >
            <v-carousel-item
                v-for="(item,i) in items"
                :key="i"
            >
              <v-slide-item>
                <v-row
                    class="fill-height"
                    align="center"
                    justify="center"
                >
                  <v-col
                      cols="6">
                    <v-img
                        min-height="450"
                        :src="item.src"
                        :href="item.link"
                    ></v-img>
                  </v-col>
                  <v-col cols="6"
                    v-for="(it, ind) in item_two"
                         :key="ind"
                  >
                    <v-img
                        :src="it.src"
                        :href="it.link"
                    ></v-img>
                  </v-col>
                </v-row>
              </v-slide-item>
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>

      <!--Lo mas buscado-->
      <v-row class="mt-5">
        <v-col
            cols="12"
        >
          <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/12/CINTILLOS/webp/cintillo_middle_desk.webp?v2"></v-img>
        </v-col>
      </v-row>
      <v-row class="mt-4">
        <v-col cols="12">
          <v-img min-width="1" src="../assets/titulo_losmasbuscados.webp"/>
        </v-col>
      </v-row>
      <v-row class="mt-4">
        <v-col cols="5" class="px-0">
          <img width="100%" height="100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/12/DESTACADOS/BLOQ1/webp/1.webp">
        </v-col>
        <v-col cols="7" class="pr-0">
          <img width="100%" height="100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/DESTACADOS/BLOQ1/webp/2.webp?v1">
        </v-col>
      </v-row>
      <v-row class="mt-4">
        <v-row>
          <v-col cols="2" class="pa-1" >
            <v-img style="height: 100%; width: 100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/DESTACADOS/BLOQ1/webp/3.webp?v1"></v-img>
          </v-col>
          <v-col cols="5" >
            <v-row class="pa-1">
              <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/DESTACADOS/BLOQ1/webp/4.webp?v1"></v-img>
            </v-row>
            <v-row class="pa-1">
              <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/DESTACADOS/BLOQ1/webp/6.webp?v1"></v-img>
            </v-row>
          </v-col>
          <v-col cols="5" >
            <v-row class="pa-1">
              <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/DESTACADOS/BLOQ1/webp/5.webp?v1"></v-img>
            </v-row>
            <v-row class="pa-1">
              <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/11/DESTACADOS/BLOQ1/webp/7.webp"></v-img>
            </v-row>
          </v-col>
        </v-row>
      </v-row>

      <!--descubre lo nuevo-->
      <h1 class=" d-flex justify-center mt-10 card_title " >
        <span class="font-weight-light">descubre .</span> <strong>  lo + nuevo</strong>
      </h1>

      <!--CARRUSEL: descubre lo nuevo-->
      <v-row>
        <v-col cols="1">
          <v-img src="../assets/lo-nuevo.webp"></v-img>
        </v-col>
        <v-col cols="11">
          <v-carousel
              v-model="model"
              cycle
              hide-delimiter-background
              show-arrows
          >
            <v-carousel-item
                v-for="(el,i) in elementos"
                :key="i"
            >
              <v-slide-item>
                <v-row
                    class="fill-height"
                    align="center"
                    justify="center"
                >
                  <v-col
                      cols="4">
                    <v-img
                        min-height="420"
                        :src="el.src"
                        :href="el.link"
                    ></v-img>
                  </v-col>
                  <v-col cols="4"
                         v-for="(elt, j) in elementos_two"
                         :key="j"
                  >
                    <v-img
                        :src="elt.src"
                        :href="elt.link"
                    ></v-img>
                  </v-col>
                </v-row>
              </v-slide-item>
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>

      <h1 class=" d-flex justify-center mt-10 card_title " >
        <span class="font-weight-light">conoce nuestras .</span> <strong> nuevas categorías.</strong>
      </h1>

      <!--Nuevas Categorias-->
      <div>
        <v-card elevation="0">
          <v-container>
            <v-row>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/NUEVAS_CATEGORIAS/webp/1.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">MASCOTAS</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0" >
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/NUEVAS_CATEGORIAS/webp/2.webp"></v-img>
                  <v-card-title  class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">MEJORAS HOGAR</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/NUEVAS_CATEGORIAS/webp/3.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">SALUD</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/NUEVAS_CATEGORIAS/webp/4.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">SUPERMERCADO</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/NUEVAS_CATEGORIAS/webp/5.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center text-center" style="font-size: 14pt; font-weight: bold">LICORES, CERVEZAS Y ACCESORIOS</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/14/NUEVAS_CATEGORIAS/webp/6.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">INTERNACIONAL</v-card-title>
                </v-card>
              </v-col>
            </v-row>
          </v-container>
        </v-card>
      </div>

      <!--Aprovecha las promociones-->
      <h1 class=" d-flex justify-center mt-10 card_title mb-5 " >
        <span class="font-weight-light">Aprovecha las .</span> <strong>promociones</strong>
      </h1>

      <v-row class="mt-4" style="height: 300pt; gap: 6pt">
        <v-col cols="2,5 pa-0" style="height: 300pt">
          <img style="height: 300pt; width: 100%"  src="https://home.ripley.com.pe/minisitios/home/c/22/07/13/DESTACADOS/BLOQ2/webp/8.webp?v1">
        </v-col>
        <v-col cols="2,5 pa-0" style="height: 300pt">
          <img style="height: 300pt; width: 100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/14/DESTACADOS/BLOQ2/webp/9.webp">
        </v-col>
        <v-col cols="4,5" style="height: 280pt">
          <v-row style="height: 150pt">
            <img  style="height: 150pt; width: 390pt" src="https://home.ripley.com.pe/minisitios/home/c/22/07/14/DESTACADOS/BLOQ2/webp/10.webp">
          </v-row>
          <v-row class="pt-2" style="height: 150pt">
            <img style="height: 144pt; width: 390pt" src="https://home.ripley.com.pe/minisitios/home/c/22/07/14/DESTACADOS/BLOQ2/webp/11.webp">
          </v-row>
        </v-col>
        <v-col cols="2,5 pa-0">
          <img style="height: 300pt; width: 100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/14/DESTACADOS/BLOQ2/webp/12.webp">
        </v-col>
      </v-row>
      <v-row class="mt-5">
        <v-col class="pa-0" cols="7">
          <img style="height: 175pt; width: 100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/13/DESTACADOS/BLOQ2/webp/13.webp?v1">
        </v-col>
        <v-col class="pl-2 pt-0 pr-0 pb-0" cols="5">
          <img style="height: 175pt; width: 100%" src="https://home.ripley.com.pe/minisitios/home/c/22/07/13/DESTACADOS/BLOQ2/webp/14.webp">
        </v-col>
      </v-row>

      <!--tus categorias favoritas-->
      <h1 class=" d-flex justify-center mt-10 card_title mb-5 " >
        <strong>tus categorías favoritas</strong>
      </h1>

      <div>
        <v-card elevation="0">
          <v-container>
            <v-row>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/1.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">MUJER</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0" >
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/2.webp"></v-img>
                  <v-card-title  class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">HOMBRE</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/3.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">CALZADO</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/4.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">BELLEZA</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/5.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center text-center" style="font-size: 14pt; font-weight: bold">INFANTIL</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/6.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">JUGUETES</v-card-title>
                </v-card>
              </v-col>
            </v-row>
          </v-container>
        </v-card>
        <v-card elevation="0">
          <v-container>
            <v-row>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/7.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">DEPORTE</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0" >
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/8.webp"></v-img>
                  <v-card-title  class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">ACCESORIOS</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/9.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">TECNOLOGÍA</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/10.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">DECOHOGAR</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/11.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center text-center" style="font-size: 14pt; font-weight: bold">ELECTRO</v-card-title>
                </v-card>
              </v-col>
              <v-col cols="2">
                <v-card elevation="0">
                  <v-img src="https://home.ripley.com.pe/minisitios/home/c/22/07/09/CATEGORIAS_TRAD/webp/12.webp"></v-img>
                  <v-card-title class="pa-0 flex justify-center" style="font-size: 14pt; font-weight: bold">DORMITORIO</v-card-title>
                </v-card>
              </v-col>
            </v-row>
          </v-container>
        </v-card>
      </div>

      <!--en marcas lo tenemos tooodo-->
      <h1 class=" d-flex justify-center mt-10 card_title mb-5 " >
        <strong>en marcas,</strong><span class="font-weight-light">. lo tenemos todo</span>
      </h1>

      <!--carrusel de marcas-->
        <v-app id="inspire mb-0" style="height: 310pt">
          <v-sheet
              class="mx-auto"
              elevation="0"
              max-width="1350"
          >
            <v-slide-group
                v-model="modal"
                class="pa-2"
                center-active
                show-arrows
            >
              <v-slide-item
                  v-for="(marca, n) in marcas"
                  :key="n"
                  v-slot="{ active, toggle }"
              >
                <!-- v-slot="{ active, toggle }" -->
                <v-card
                    :color="active ? 'primary' : 'grey lighten-1'"
                    class="ma-1"
                    height="325"
                    width="197"
                    @click="toggle"
                >
                  <v-img
                      height="325"
                      :src="marca.src"
                  >
                  </v-img>
                  <!-- @click="toggle" -->
                  <!-- -->
                  <!--
                  <v-row
                      class="fill-height"
                      align="center"
                      justify="center"
                  >

                    <v-scale-transition>
                      <v-icon
                          v-if="active"
                          color="red"
                          size="48"
                          v-text="'mdi-close-circle-outline'"
                      >
                      </v-icon>
                    </v-scale-transition>
                  </v-row>
                  -->
                </v-card>
              </v-slide-item>
            </v-slide-group>
          </v-sheet>
        </v-app>

      <!--emprendedores y pymes-->
      <h1 class=" d-flex justify-center mt-10 card_title mb-5 " >
        <strong>emprendedores y pymes</strong>
      </h1>

      <v-row>
        <v-col cols="1 pt-7 pb-7">
          <img height="485" src="https://home.ripley.com.pe/minisitios/home/c/22/05/06/EMPRENDEDORES/webp/emprendedores_titulo.webp">
        </v-col>
        <v-col cols="11">
          <v-carousel
              v-model="model"
              cycle
              hide-delimiter-background
              show-arrows
          >
            <v-carousel-item
                v-for="(el,i) in elementos"
                :key="i"
            >
              <v-slide-item>
                <v-row
                    class="fill-height"
                    align="center"
                    justify="center"
                >
                  <v-col
                      cols="4">
                    <v-img
                        min-height="420"
                        :src="el.src"
                        :href="el.link"
                    ></v-img>
                  </v-col>
                  <v-col cols="4"
                         v-for="(elt, j) in elementos_two"
                         :key="j"
                  >
                    <v-img
                        :src="elt.src"
                        :href="elt.link"
                    ></v-img>
                  </v-col>
                </v-row>
              </v-slide-item>
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>



    </v-container>
  </div>
</template>

<script lang="ts">
import {  Ref, ref, defineComponent} from "@vue/composition-api";

//import { Carousel, Slide } from 'vue-carousel';

export default defineComponent({
  name: "MainSection",
  /**
   components  : {
      Carousel,
      Slide
    },
   */
  setup: function () {

    //Variables
    const slide: Ref<number> = ref(0);
    const sliding: Ref<any> = ref(null);

    const model: Ref<number> = ref(0);
    /** Arrays para Carrusel de mascotas */
    const items: Ref<Array<any>> = ref([
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/1.jpg',
        link: 'https://simple.ripley.com.pe/mujer/ropa-mujer/ver-todo'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/2.jpg',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/3.jpg?v2',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      }
    ]);

    const item_two: Ref<Array<any>> = ref([
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/2.webp',
        link: 'https://simple.ripley.com.pe/mujer/ropa-mujer/ver-todo'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/4.webp',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/6.webp',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      }
    ]);

    /** Arrays para Carrusel de "descubre lo + nuevo" */
    const elementos: Ref<Array<any>> = ref([
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/13/LO_MAS_NUEVO/webp/1.webp',
        link: 'https://simple.ripley.com.pe/mujer/ropa-mujer/ver-todo'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/LO_MAS_NUEVO/webp/2.webp',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/LO_MAS_NUEVO/webp/3.webp',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      }
    ]);

    const elementos_two: Ref<Array<any>> = ref([
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/2.webp',
        link: 'https://simple.ripley.com.pe/mujer/ropa-mujer/ver-todo'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/4.webp',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/ZONA_CAMPANAS/webp/6.webp',
        link: 'https://simple.ripley.com.pe/hogar/ropa-de-cama/edredones-y-sets-de-cama-deco'
      }
    ]);



    const modal: Ref<any> = ref(0);

    const marcas: Ref<Array<any>> = ref([
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/1.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/2.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/3.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/4.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/5.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/13/SIS/webp/6.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/7.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/8.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/10.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/11.webp',
      },
      {
        src: 'https://home.ripley.com.pe/minisitios/home/c/22/07/09/SIS/webp/12.webp?v1',
      }
    ])

    const onSlideStart = (slide: any) => {
      sliding.value = true
    }

    const onSlideEnd = (slide: any) => {
      sliding.value = false
    }

    return {
      //variables
      model,
      modal,
      marcas,
      items,
      item_two,
      slide,
      sliding,
      elementos,
      elementos_two,

      //methods
      onSlideStart,
      onSlideEnd
    }

  }
})
</script>

<style scoped>
.card_title{
  font-size: 35px;
  color: #4a4a4a ;
}
@media (min-width: 1048px) {
  /**1024*/
  .container {
    /**1350*/
    max-width: 1450px !important;
  }
}
</style>