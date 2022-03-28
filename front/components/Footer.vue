<template>
<div>
    <!-- <img src="../assets/img/orange.png" width="80px"> -->
    <v-footer color="#FAF6ED" fixed app>
      <div class="nav">
        <NuxtLink to="/"><div class="menu">Works</div></NuxtLink>
        <NuxtLink to=""><div class="menu">Friends</div></NuxtLink>
        <NuxtLink to=""><div class="menu">Profile</div></NuxtLink>
      </div>
    </v-footer>
</div>
</template>

<script>
export default {

}
</script>

<style>
.nav {
 margin-right: auto;
 margin-left: auto;
 align-items: center; 
}
.menu{
  float: left;
  padding: 10px 20px;
  font-size: 20px;
}
</style>