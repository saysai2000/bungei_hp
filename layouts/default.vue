<template>
  <v-app dark>
    <v-app-bar
      color="deep-purple accent-4"
      dense
      dark
    >
      <span>
        <v-btn
          color="secondary"
          fab
          small
        >文</v-btn>
      </span>

      <v-spacer></v-spacer>

      <v-tabs
        fixed-tabs
        background-color="indigo"
        dark
        >
        <v-tab>
          文芸部とは
        </v-tab>
        <v-tab>
          作品
        </v-tab>
        <v-tab>
          年表
        </v-tab>
        <v-tab>
          SNS
        </v-tab>
      </v-tabs>

      <v-btn
        color="secondary"
        fab
        small
      >🔎</v-btn>
      <v-btn
        color="secondary"
        fab
        small
      >🛒</v-btn>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
