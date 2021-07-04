<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
      extended
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />
      </div>
      <v-toolbar-title>Vueshop</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon to="/about">
        <v-badge color="orange" overlap>
          <template v-slot:badge>
              <span>3</span>
            </template>
          <v-icon>
            mdi-cart
          </v-icon>
        </v-badge>
      </v-btn>

      <v-text-field
        slot="extension"
        hide-details
        append-icon="mdi-microphone"
        flat
        label="search"
        prepend-inner-icon="mdi-magnify"
        solo-inverted
      ></v-text-field>
    </v-app-bar>

    <v-main>
      <v-content>
        <v-container fluid>
          <router-view></router-view>
        </v-container>
      </v-content>
      <!-- <HelloWorld/> -->
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    // HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
