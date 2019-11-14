<template>
  <v-app>
    <v-app-bar
      app
      color="black"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Film-It Logo"
          class="shrink mr-2"
          contain
          src="@/assets/Popcorn.png"
          transition="scale-transition"
          width="40"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2" >Inicio</span>
      </v-btn>
      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2" >Nosotros</span>
      </v-btn>
      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2" >Contacto</span>
      </v-btn>
      <v-btn
        rounded
        primary
        color="#EBC700"
      >
        <span class="mr-2" >Iniciar Sesion</span>
      </v-btn>
    </v-app-bar>

    <v-content class="mx-5">
      <Home></Home>
    </v-content>
  </v-app>
</template>

<style lang="scss" scoped>
#app{
  background-color: #9B0000;
}
</style>

<script>
import Home from '@/views/Home.vue';

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    items: [
      { name: 'Inicio' },
      { name: 'Nosotros' },
      { name: 'Contacto' },
    ],
  }),
};
</script>
