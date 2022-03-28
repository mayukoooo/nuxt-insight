<template>
  <div>
    <v-app-bar class="head" fixed app>
      <NuxtLink to="/">
        <div class="logo">
            <img src="~/assets/img/logo.png" width="90px">
        </div>
      </NuxtLink>
      <v-spacer />

      <NuxtLink to="/review">
        <v-col class="icon" cols="12" sm="2">
            <img src="~/assets/img/myworks_icon.png" width="40px">
        </v-col>
      </NuxtLink>
    </v-app-bar>
    
    <v-main>
      <v-container class="container">
        <Nuxt />
      </v-container>
    </v-main>
    
    <div>
      <Footer />
    </div>
  </div>
</template>

<script>
</script>

<style>
.container {
  background-image: linear-gradient(to right, #ffecd2 0%, #fcb69f 100%);
  /* background-image: url("../assets/img/background.png"); */
}
.logo {
  /* margin-right: auto;
  margin-left: auto;
  align-items: center; */
  text-align: center;
}
.head {
  padding: 4px;
}
/* .icon {
  background-image: url("../assets/img/kiiro.png");
  width: 80px;
} */
</style>

