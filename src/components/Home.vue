<template>
  <v-container fill-height fluid>
    <v-row class="text-center">
      <v-col cols="12">
        <v-avatar size="150">
      <img
        src="@/assets/my_avatar.jpeg"
        alt="Abhilash"
      >
    </v-avatar>
      </v-col>

      <v-col class="mb-4">
        <h4 class="display-2 font-weight-bold mb-3">
          Abhilash Kulkarni
        </h4>

        <p class="subheading font-weight-regular">
         I'm a Data Scientist &#128200; <br/>
         and a Full Stack Developer &#128187;
        </p>
      </v-col>

      <!-- <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          What's next?
        </h2>

        <v-row justify="center">
          <a
            v-for="(next, i) in whatsNext"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>
        </v-row>
      </v-col> -->

    

    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Home',

    data: () => ({
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/getting-started/pre-made-layouts', 
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>
