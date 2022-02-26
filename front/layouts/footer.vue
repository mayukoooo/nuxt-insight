<template>
  <v-app>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer :absolute="fixed"
      app>
      <NuxtLink to="/works"><v-btn>
        <span>Works</span>

        <v-icon>mdi-television-play</v-icon>
      </v-btn></NuxtLink>

      <NuxtLink to="/profile"><v-btn>
        <span>Profile</span>

        <v-icon>mdi-music-note</v-icon>
      </v-btn></NuxtLink>
    </v-footer>
    </v-app>
  </template>

<script>
export default {
  data(){
    return{
      fixed: true,
    }
  }
}
</script>

<style>
/* .nav {
  display: flex;
  justify-content: space-around;
}

.item{
  font-size: 20px;
  margin: 10px;
  padding: 10px;
} */
</style>