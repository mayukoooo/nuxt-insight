<template>
  <v-app dark>
    <!-- <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >

        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->
    <v-app-bar fixed app>
      <NuxtLink to="/"><v-toolbar-title v-text="title" /></NuxtLink>
      <v-spacer />
      <NuxtLink to="/review">
      <v-col cols="12" sm="2">
        <v-btn icon color="#FFAB91">
          <v-icon>mdi-heart</v-icon>
        </v-btn>
      </v-col>
      </NuxtLink>
    </v-app-bar>
    
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <!-- <v-navigation-drawer
      v-model="rightDrawer"
      :right="right"
      temporary
      fixed
    >
      <v-list>
        <v-list-item @click.native="right = !right">
          <v-list-item-action>
            <v-icon light>
              mdi-repeat
            </v-icon>
          </v-list-item-action>
          <v-list-item-title>Switch drawer (click me)</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->

    <!-- <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer> -->

  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      // clipped: false,
      // drawer: false,
      // fixed: false,
      // items: [
      //   {
      //     icon: 'mdi-apps',
      //     title: 'Welcome',
      //     to: '/'
      //   },
      //   {
      //     icon: 'mdi-chart-bubble',
      //     title: 'Inspire',
      //     to: '/inspire'
      //   }
      // ],
      // miniVariant: false,
      // right: true,
      // rightDrawer: false,
      title: 'Insight'
    }
  }
}
</script>

