<template>
  <v-app>
    <router-view name="toolbar" />
    <v-main>
      <router-view :key="$route.fullPath"/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import {defineComponent} from "@vue/composition-api";

export default defineComponent({
  name: 'App',

   setup (){
    //...
   }
})
</script>
