<template>
  <v-row>
    <v-col
      cols="12"
      sm="6"
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
          height="350"
          max-width="350"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            価値観
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>
    </v-col>

    <v-col
      cols="12"
      sm="6"
    >
      <v-hover
        v-slot="{ hover }"
        close-delay="100"
      >
        <NuxtLink to="/work/1/create">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="350"
          max-width="350"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            情熱
            <v-spacer></v-spacer>
            <p>説明説明説明説明</p>
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>
    </v-col>

    <v-col
      cols="12"
      sm="6"
    >
      <v-hover
        v-slot="{ hover }"
        open-delay="100"
      >
        <NuxtLink to="/work/2/create">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="350"
          max-width="350"
        >
          <v-card-text class="font-weight-medium mt-12 text-center text-subtitle-1">
            情熱
          </v-card-text>
        </v-card>
        </NuxtLink>
      </v-hover>
    </v-col>

    <v-col
      cols="12"
      sm="6"
    >
      <v-hover
        v-slot="{ hover }"
        open-delay="100"
      >
        <NuxtLink to="/work/3/create">
        <v-card
          :elevation="hover ? 16 : 2"
          :class="{ 'on-hover': hover }"
          class="mx-auto"
          height="350"
          max-width="350"
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

</style>