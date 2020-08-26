<template>
  <v-app>
    <!-- <v-app-bar
      app
      flat
      dense
      color="white"
    >

      <v-spacer></v-spacer>
        <v-btn class="ma-2" tile color="indigo" dark small outlined>Profile
        <v-icon dark right>mdi-emoticon-cool</v-icon>
        </v-btn>
        <v-btn class="ma-2" tile color="indigo" dark small outlined>Projects
        <v-icon dark right>mdi-laptop-chromebook</v-icon>
        </v-btn>
    </v-app-bar> -->

    <v-main>
      <Home/>
    </v-main>
    <v-footer padless class="indigo white--text lighten-1">
    <v-col
      class="text-center"
      cols="12"
    >
      <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
    </v-col>
  </v-footer>
  </v-app>
</template>

<script>
import Home from './components/Home';

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    icons: [
        'mdi-facebook',
        'mdi-github',
        'mdi-linkedin',
        'mdi-instagram',
      ],
  }),
};
</script>
