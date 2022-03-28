<template>
  <v-app-bar fixed app>
    <NuxtLink to="/"><v-toolbar-title v-text="title" /></NuxtLink>
    <v-spacer />
    <NuxtLink to="/review">
    <v-col cols="12" sm="2">
      <v-btn icon color="#FFAB91">
        <v-img
        src="../assets/img/myworks_icon.png"
        ></v-img>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
    </v-col>
    </NuxtLink>
  </v-app-bar> 
</template>

<script>
export default {

}
</script>

<style>

</style>