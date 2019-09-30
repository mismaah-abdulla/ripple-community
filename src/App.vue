<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <a href="/">
        <span class="primary--text">RIPPLE</span>
        <span class="font-weight-light black--text">COMMUNITY</span>
        </a>
      </v-toolbar-title>
      <v-spacer></v-spacer>

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
        href="/"
      >
        <span class="mr-2">Forum</span>
      </v-btn>
      <v-btn
        text
        href="#/about"
      >
        <span class="mr-2">About</span>
      </v-btn>
      <v-btn
        text
        href="#/contactus"
      >
        <span class="mr-2">Contact Us</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <router-view></router-view>
    </v-content>
    <v-footer
    dark
    padless
    >
    <v-card width="100%"
      flat
      tile
      class="black white--text text-center"
    >
      <v-card-text class="pb-0">
        <v-btn
          v-for="contact in contacts"
          :key="contact.id"
          class="mx-4 white--text"
          icon
          v-bind:href="contact.link" target="_blank"
        >
          <v-icon size="24px">{{ contact.icon }}</v-icon>
        </v-btn>
      </v-card-text>
      <v-card-text>
        <a href="#/legal" style="color : #e6e6e6;">Terms of Use & Privacy Policy</a>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="primary--text">
        {{ new Date().getFullYear() }} — <strong>Ripple Community</strong>
      </v-card-text>
    </v-card>
  </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  components: {
  },
  data: () => ({
    contacts: [
      { id: 1, icon: 'mdi-facebook', link: 'https://www.facebook.com/ripplecommunity.space/' },
      { id: 2, icon: 'mdi-youtube', link: 'https://www.youtube.com/channel/UCwH3qttuVdHARTyZaZXQqOw' },
      { id: 3, icon: 'mdi-instagram', link: 'https://www.instagram.com/ripple.community/' }
    ]
  })
}
</script>

<style>
a {
  color: inherit;
  text-decoration: none;
}
</style>
