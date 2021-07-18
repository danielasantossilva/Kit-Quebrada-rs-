<template>
  <v-app>
  <app-top-bar/>

    <v-main>
      <Inicio/>        
    </v-main>
  </v-app>
</template>

<script>
import Inicio from './components/Inicio.vue'
import AppTopBar from './components/Shered/AppTopBar.vue'

export default {
  name: 'App',
  components: {
  Inicio,
    AppTopBar

  }
  };
</script>

<style scoped>

</style>