<template>
  <!-- <HelloWorld /> -->
  <v-container pa-0>
    <v-parallax id="parallax-ripple"
      dark
      height="500"
      src="/ripple-effect.jpg"
    >
      <v-row
        align="center"
        justify="start"
      >
        <h1 class="display-3 mb-4 secondary--text">Mental Health & Self Help <br/> Wisdom & Inspiration <br/> Life Style & Well being</h1>
      </v-row>
    </v-parallax>
    <v-row justify="center">
      <v-card><img src="/logo.webp"></v-card>
      
    </v-row>
  </v-container>
</template>

<style>
  /* #parallax-ripple img {
    height: 100%
  } */
</style>


<script>
// import HelloWorld from '../components/HelloWorld'

export default {
  components: {
    // HelloWorld
  }
}
</script>
