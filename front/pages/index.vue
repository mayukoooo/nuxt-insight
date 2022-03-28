<template>
  <v-row class="home" justify="center" align-content="center">
    <!-- <v-col
      cols="12"
      sm="6"
    > -->
    <v-col
      cols="6"
    >
      <v-hover
        v-slot="{ hover }"
        open-delay="100"
      >
        <NuxtLink to="/work/0/create">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="150"
          max-width="150"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            価値観
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>
    
      <v-hover
        v-slot="{ hover }"
        close-delay="100"
      >
        <NuxtLink to="">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="150"
          max-width="150"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            情熱
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>
 
      <v-hover
        v-slot="{ hover }"
        open-delay="100"
      >
        <NuxtLink to="">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="150"
          max-width="150"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            情熱
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>

      <v-hover
        v-slot="{ hover }"
        open-delay="100"
      >
        <NuxtLink to="">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="150"
          max-width="150"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            フィット
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>
    </v-col>

  </v-row>
</template>

<script>
export default {

}
</script>

<style>
.home {
  width: 100%;
	height: 100vh;
  background-size: cover;
  background-size: 200% 200%;
}
</style>