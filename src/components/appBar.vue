<template>
  <v-app-bar
      color="#1a1a1a"
      flat
      :height="cardHeight"
      :width="cardWidth"
  >
    <v-container fluid
    >
      <v-row no-gutters class="mt-2">
        <v-col
            cols="1"
        >
          <v-toolbar-title class="pl-8">
            <v-img class="float-left d-none d-md-block"
                   src="https://home.ripley.com.pe/pets/ripley-pets.gif"
                   max-width="50"
                   width="50"
                   max-height="50"/>
          </v-toolbar-title>
        </v-col>
        <v-col
            cols="2"
        >
          <div style="display: flex; justify-content: flex-start">
              <v-btn
              color="#70578b"
              fab
              dark
              width="45"
              height="45"
              style="margin-right: 10pt"
              >
              <v-icon>mdi-menu mdi-36px</v-icon>
              </v-btn>
              <div>
              <span style="color: #ffffff; font-weight: bold">Menú de<br>Categorías</span>
              </div>
          </div>
        </v-col>
        <v-col
            cols="6"
        >
          <v-text-field
              flat
              solo
              hide-details
              :label="$t('Buscar productos')"
              v-model="txtSearchProduct"
              @keyup.enter="onSearch"
              class="rounded-r-0"
          >
          </v-text-field>
        </v-col>
        <v-col>
          <v-btn
              height="48"
              color="#848484"
              dark
              class="rounded-l-0"
              elevation="0"
          >
            <v-icon
                large
            >mdi-magnify
            </v-icon>
          </v-btn>
        </v-col>
        <v-col
            cols="1"
            md="1"
        >

          <v-btn
              color="#fff"
              icon
              style="margin-left: 40pt"
          >
            <span>Bienvenid@<br>
            Iniciar Sesión
            <v-icon>mdi-chevron-up</v-icon>
            </span>
          </v-btn>
        </v-col>
        <v-col
          cols="1"
          style="text-align: center"
        >
          <v-btn
              icon
          >
            <a href="#" style="text-decoration: none">
              <v-icon
                  large
                  color="#fff"
              >
                mdi-purse-outline
              </v-icon>
            </a>
          </v-btn>
        </v-col>

      </v-row >
    </v-container>
  </v-app-bar>
</template>


<script lang="ts">

import { ref, defineComponent, SetupContext } from "@vue/composition-api";
import i18n from "@/plugins/i18n";
import { WebPages } from "@/constants";

export default defineComponent({
  name: 'appBar',
  computed:
      {
        cardWidth() {
          switch (this.$vuetify.breakpoint.name) {
            case 'xs':
              return '100%'
          }
        },
        cardHeight() {
          switch (this.$vuetify.breakpoint.name) {
            case 'xs':
              return '87px'
            case 'sm':
              return '87px'
            case 'md':
              return '87px'
            case 'lg':
              return '87px'
            case 'xl':
              return '100px'
          }
        }
      },

  setup(_, context: SetupContext){
    const e1 = 'es';

    const txtSearchProduct =  ref();

    const lang = [
      { id: 'es', title: 'Español', iconlang:'https://upload.wikimedia.org/wikipedia/commons/thumb/c/ce/Flag_of_Catalonia.svg/2560px-Flag_of_Catalonia.svg.png' },
      { id: 'en', title: 'Ingles', iconlang:'https://www.nicepng.com/png/full/6-63506_usa-png-clipart-american-flag-icon-png.png'}
    ];
    function selectLanguage(id:string) {
      i18n.locale = id;

    }
    const onSearch = async ()  => {
      if(txtSearchProduct.value.trim().length <= 0 ) return;

      context.root.$router.push({
        name: WebPages.PRODUCTVIEW,
        query: {
          nompro: txtSearchProduct.value
        }
      }).catch(e => console.log("Error-Navbar: ",e));
    }
    return {
      e1,
      lang,
      txtSearchProduct,
      selectLanguage,
      onSearch,
    }


  }
})
</script>

<style>
.v-toolbar__content, .v-toolbar__extension {
  padding: 0px;
}
.container {
  padding: 0;
}
.v-toolbar__content .v-btn.v-btn--icon.v-size--default, .v-toolbar__extension .v-btn.v-btn--icon.v-size--default {
  height: 48px;
  width: 0;
}
@media (min-width: 1024px) {
  .container {
    max-width: 900px;
  }
}
@media (max-width: 1920px) {
  .container {
    max-width: 85%;
  }
}
@media (max-width: 1250px) {
  .container {
    max-width: 100%;
  }
}
.category-color{
  color: rgba(51,51,51,.6) !important;
}
.category-color2{
  color: #333333 !important;
}
.carousel-container .next-button, .carousel-container .prev-button {
  width: 64px;
  height: 64px;
  /* display: none; */
  background-color: #fff;
  /* border-radius: 50%; */
  border-width: 0;
  box-shadow: 0 2px 4px 0 rgb(0 0 0 / 19%);
  cursor: pointer;
  outline: 0;
  position: absolute;
  top: 48%;
  z-index: 2;
}
</style>