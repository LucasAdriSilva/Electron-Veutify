<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-toolbar-tittle> Unspecified Project</v-toolbar-tittle>
    </v-app-bar>

    <v-main>
    <Home/>
    </v-main>
  </v-app>
</template>

<script>
import Home from './components/Home.vue';

export default {
  name: 'App',

  components: { 
    Home,
  },

  data: () => ({
    //
  }),
};
</script>
