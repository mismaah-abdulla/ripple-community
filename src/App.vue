<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>RIPPLE</span>
        <span class="font-weight-light">COMMUNITY</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        text
        href="#/about"
      >
        <span class="mr-2">About</span>
      </v-btn>
      <v-btn
        text
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
      >
        <span class="mr-2">Self Care</span>
      </v-btn>
      <v-btn
        text
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
      >
        <span class="mr-2">Suicide Prevention</span>
      </v-btn>
      <v-btn
        text
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
      >
        <span class="mr-2">Support Group</span>
      </v-btn>
      <v-btn
        text
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
      >
        <span class="mr-2">Contact Us</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
    //
  }),
};
</script>
