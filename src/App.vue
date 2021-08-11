<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <v-toolbar-title>Page title</v-toolbar-title>
    <v-spacer/>
    <v-btn icon to="/">
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-btn icon to="/about">
        <v-icon>mdi-heart</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </v-app-bar>
    <v-content>
      <router-view/>
    </v-content>
    <v-footer app absolute class="font-weight-medium">
      <v-col
        class="text-center"
        cols="12"
      >
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-col>
    </v-footer>
  </v-app>
</template>

<script>

export default {
  name: 'App'

}
</script>
