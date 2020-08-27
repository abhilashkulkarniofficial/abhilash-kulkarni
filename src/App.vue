<template>
  <v-app>
    
    <v-main>
      <Home/>
    </v-main>

    <v-footer padless color="white">
    <v-col
      class="text-center"
      cols="12"
    >
    <v-btn
          v-for="(item, index) in icons"
          :key="index"
          class="mx-4 gray--text"
          icon
          :href="item.link"
          target="_blank"
        > 
          <v-icon size="24px">{{ item.icon }}</v-icon>
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
      {
        icon:'mdi-facebook',
        link:'https://www.facebook.com/kulluabhi/'
      },
      {
        icon:'mdi-github',
        link:'https://github.com/abhilashkulkarniofficial'
      },
      {
        icon:'mdi-linkedin',
        link:'https://www.linkedin.com/in/abhilashkulkarniofficial/'
      },
      {
        icon:'mdi-instagram',
        link:'https://www.instagram.com/the_koolkarni/'
      }
      ],
  }),
};
</script>
