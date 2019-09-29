<template>
  <v-container>
      <v-row justify="center" class="py-5">
          <h1 class="headline">Make ripples with us!</h1>
      </v-row>
      <v-row justify="center">
          <h1 class="subtitle-1">Contact us at <a href="mailto:ripple.theteam@gmail.com" target="_blank" style="text-decoration : none;">ripple.theteam@gmail.com</a></h1>
      </v-row>
      <v-row justify="center">
        <h1 class="subtitle-1">Or message us on social media!</h1>
      </v-row>
      <v-row justify="center">
        <v-card>
            <v-card-text>
                <v-btn x-large
                v-for="contact in contacts"
                :key="contact.id"
                class="mx-4 primary--text"
                icon
                v-bind:href="contact.link" target="_blank"
                >
                <v-icon x-large>{{ contact.icon }}</v-icon>
                </v-btn>
            </v-card-text>
          </v-card>
      </v-row>
  </v-container>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data: () => ({
    contacts: [
        {id: 1, icon: 'mdi-facebook', link: "https://www.facebook.com/ripplecommunity.space/"},
        {id: 2, icon: 'mdi-youtube', link: "https://www.youtube.com/channel/UCwH3qttuVdHARTyZaZXQqOw"},
        {id: 3, icon: 'mdi-instagram', link: "https://www.instagram.com/ripple.community/"}
      ],
  })
}
</script>