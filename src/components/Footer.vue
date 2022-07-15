<template>
  <div>
      <div style="background-color: #eeeeee; display: flex; justify-content: center; align-items: center; height: 40pt">
        <v-btn plain style="font-size: 15pt; color: #7E57C2"><v-icon >mdi-chevron-up mdi-36px</v-icon> subir</v-btn>
      </div>
    <!--Beneficios de Ripley-->
    <div class="deep-purple lighten-1"> <!--solo para el color violeta-->
      <div class="container"> <!--Contenedor del ancho-->
      <v-row style="height: 150pt">
        <v-col cols="2" class="pt-9">
          <v-card
              color="transparent"
              class="mx-auto text-center"
              elevation="0"
              max-width="344"
          >
            <v-btn
                text
                color="deep-purple accent-4"
            >
              <v-img src="https://home.ripley.com.pe/minisitios/home/d/iconos/retiro-en-tienda.svg"></v-img>
            </v-btn>
            <v-card-text>
              <p class="text-h6 mb-0" style="color: #ffffff">
                Retiro en Tienda
              </p>
              <div style="color: #ffffff; font-size: 12pt">
                Más de 30 tiendas a lo<br>
                largo del Perú
              </div>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="2" class="pt-9">
          <v-card
              color="transparent"
              class="mx-auto text-center"
              elevation="0"
              max-width="344"
          >
            <v-btn
                text
                color="deep-purple accent-4"
            >
              <v-img src="https://home.ripley.com.pe/minisitios/home/d/21/02/24/btn5-v2.svg"></v-img>
            </v-btn>
            <v-card-text>
              <p class="text-h6 mb-0" style="color: #ffffff">
                Agención al Cliente
              </p>
              <div style="color: #ffffff; font-size: 12pt">
                <v-icon dark>mdi-whatsapp</v-icon> +51 941955900<br>
                (01) 611-5959
              </div>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="2" class="pt-9">
          <v-card
              color="transparent"
              class="mx-auto text-center"
              elevation="0"
              max-width="344"
          >
            <v-btn
                text
                color="deep-purple accent-4"
            >
              <img height="90pt" src="https://home.ripley.com.pe/minisitios/home/d/iconos/extra-garantia.svg">
            </v-btn>
            <v-card-text>
              <p class="text-h6 mb-0" style="color: #ffffff">
                Extraganrantía
              </p>
              <div style="color: #ffffff; font-size: 12pt">
                Prolonga la garantía<br>
                de tus productos
              </div>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="2" class="pt-9">
          <v-card
              color="transparent"
              class="mx-auto text-center"
              elevation="0"
              max-width="344"
          >
            <v-btn
                text
                color="deep-purple accent-4"
            >
              <img height="65pt" src="https://home.ripley.com.pe/minisitios/home/d/iconos/devolucion.svg">
            </v-btn>
            <v-card-text>
              <p class="text-h6 mb-0" style="color: #ffffff">
                Devolución
              </p>
              <div style="color: #ffffff; font-size: 12pt">
                Cambios y <br>
                Devoluciones
              </div>
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="2" class="text-center pt-12">
          <img height="100pt" src="https://home.ripley.com.pe/minisitios/home/artes/libro_reclamaciones.jpeg">
        </v-col>
        <v-col cols="2" class="pt-15">
          <v-card
              color="transparent"
              class="mx-auto text-center"
              elevation="0"
              max-width="344"
          >
            <v-btn
                text
                color="deep-purple accent-4"
            >
              <img height="65pt" src="https://home.ripley.com.pe/minisitios/home/d/iconos/servicio-al-cliente.svg">
            </v-btn>
            <v-card-text>
              <p class="text-h6 mb-0" style="color: #ffffff">
                Servicio al Cliente
              </p>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
      </div>
    </div>
    <!--Beneficios de Ripley  Zona GRIS-->
    <div style="background-color: #333333">
      <div class="container">
        <v-row style="height: 400pt">
          <v-col cols="3 mt-15">
            <v-card
                color="transparent"
                elevation="0"
            >
              <v-card-title class="pl-0 white--text font-weight-bold">Compra con Confianza</v-card-title>
              <p class="white--text mb-2" style="font-size: 13pt">¿Cómo comprar en Ripley.com?</p>
              <p class="white--text mb-2" style="font-size: 13pt">Guias de Compra</p>
              <p class="white--text mb-2" style="font-size: 13pt">Términos y codiciones</p>
              <p class="white--text mb-2" style="font-size: 13pt">Cambios y Devoluciones</p>
              <p class="white--text mb-2" style="font-size: 13pt">Bases Legales</p>
              <p class="white--text mb-2" style="font-size: 13pt">Seguridad y Privacidad</p>
              <p class="white--text mb-2" style="font-size: 13pt">Seguimiento de despacho</p>
              <p class="white--text mb-2" style="font-size: 13pt">Política de privacidad de datos</p>
            </v-card>
          </v-col>
          <v-col cols="2 mt-15">
            <v-card
                color="transparent"
                elevation="0"
            >
              <v-card-title class="pl-0 white--text font-weight-bold">Sobre Ripley</v-card-title>
              <p class="white--text mb-2" style="font-size: 13pt">Portal de Personas</p>
              <p class="white--text mb-2" style="font-size: 13pt">¿Quiénes Somos?</p>
              <p class="white--text mb-2" style="font-size: 13pt">Nuestras Tiendas</p>
              <p class="white--text mb-2" style="font-size: 13pt">Trabaka con Nosotros</p>
              <p class="white--text mb-2" style="font-size: 13pt">Comprobante Electrónico</p>
              <p class="white--text mb-2" style="font-size: 13pt">Reporte de Sostenibilidad</p>
            </v-card>
          </v-col>
          <v-col cols="3 mt-15">
            <v-card
                color="transparent"
                elevation="0"
            >
              <v-card-title class="pl-0 white--text font-weight-bold">Más de Ripley</v-card-title>
              <p class="white--text mb-2" style="font-size: 13pt">Banco Ripley</p>
              <p class="white--text mb-2" style="font-size: 13pt">Tarjeta Ripley</p>
              <p class="white--text mb-2" style="font-size: 13pt">Efectivo Express</p>
              <p class="white--text mb-2" style="font-size: 13pt">RipleyPuntos</p>
              <p class="white--text mb-2" style="font-size: 13pt">Seguros Ripley</p>
              <p class="white--text mb-2" style="font-size: 13pt">Extra Garantía</p>
              <p class="white--text mb-2" style="font-size: 13pt">Cyber Wow</p>
              <p class="white--text mb-2" style="font-size: 13pt">Cyber Day chile</p>
              <p class="white--text mb-2" style="font-size: 13pt">Ripley Chile</p>
            </v-card>
          </v-col>
          <v-col cols="4 mt-15">
            <v-card
                color="transparent"
                elevation="0"
            >
              <v-card-title class="pl-0 white--text font-weight-bold">Suscríbete</v-card-title>

              <v-row class="flex-start">
              <v-text-field
                 style="width: 250pt"
                 background-color="#fff"
                 class="pl-3 mx-0 rounded-r-0"
                 flat
                 label="Ingresa tu correo"
                 solo-inverted
              ></v-text-field>
              <v-btn elevation="0" class="rounded-l-0" style="height: 36pt" color="#8755ba" dark>Suscríbite</v-btn>
              </v-row>
              <v-row>
                <v-checkbox class="mt-0 pt-0">
                    <!--
                    v-model="checkbox"
                    :label="`Checkbox 1: ${checkbox.toString()}`"
                    -->
                </v-checkbox>
                <p class="white--text mb-2" style="font-size: 13pt">Acepto los Términos y condiciones</p>
              </v-row>
              <v-card-title class="pl-0 white--text font-weight-bold pb-5">Medios de Pago</v-card-title>
              <v-row>
                <v-icon class="ml-2 white--text">mdi-card-account-phone mdi-36px</v-icon>
                <v-icon class="ml-2 white--text">mdi-security mdi-36px</v-icon>
                <v-icon class="ml-2 white--text">mdi-credit-card mdi-36px</v-icon>
                <v-icon class="ml-2 white--text">mdi-card-bulleted-settings mdi-36px</v-icon>
                <v-icon class="ml-2 white--text">mdi-card-text mdi-36px</v-icon>
                <v-icon class="ml-2 white--text">mdi-card-account-details mdi-36px</v-icon>
              </v-row>
              <v-card-title class="pl-0 pb-3 mt-6 white--text font-weight-bold">Síguenos</v-card-title>
              <v-icon class="white--text">mdi-facebook mdi-36px</v-icon>
              <v-icon class="ml-2 white--text">mdi-twitter mdi-36px</v-icon>
              <v-icon class="ml-2 white--text">mdi-youtube mdi-36px</v-icon>
            </v-card>
          </v-col>
        </v-row>
        <v-row class="justify-center">
          <p class="white--text" style="font-size: 11pt">Por tu seguridad, recuerda revisar siempre en tu navegador que el sitio que visitas sea la versión oficial. La dirección https://simple.ripley.com.pe es la única del sitio oficial de Ripley.</p>
        </v-row>
        <v-row class="justify-center">
          <p class="grey--text text-center pb-10" style="font-size: 11pt">Precios solo disponibles en www.ripley.com.pe y Fonocompras. Precios Internet publicados incluyen descuento adicional. Precios sujetos a variaciones sin previo aviso. Productos sujetos a
          <br>disponibilidad de stock. Solo consumo familiar. Stock mínimo 1 unidad por producto. Ofertas se rigen de acuerdo a los términos y condiciones. Despacho de producto se realizará una vez
          <br>confirmada la compra.</p>
        </v-row>
      </div>
    </div>
  </div>
</template>
<script>
</script>
<style>
@media (min-width: 1048px) {
  /**1024*/
  .container {
    /**1350*/
    max-width: 1450px !important;
  }
}
</style>