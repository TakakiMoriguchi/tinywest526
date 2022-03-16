<template>
  <header class="appBar">
    <v-app-bar
      app
      dark
    >
      <v-toolbar-title>
        <nuxt-link to="/" class="siteTitle">
          <img src="/images/logo.svg" />
          <h1>tinyWEST</h1>
        </nuxt-link>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon @click="drawer=true"></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      fixed
      temporary
      right
    >
      <v-list
        nav
        dense
      >
        <div @click="drawer=false" class="closeButton"><span class="batsu"></span></div>
        <v-list-item-group>
          <v-list-item>
            <v-list-item-title><nuxt-link to="#">NEWS</nuxt-link></v-list-item-title>
          </v-list-item>
          <v-list-group>
            <template v-slot:activator>
              <v-list-item-title>ABOUT</v-list-item-title>
            </template>
            <v-list-item-content>
              <v-list-item-title class="aboutChild">DISPLAY</v-list-item-title>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-title class="aboutChild">BATTERY</v-list-item-title>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-title class="aboutChild">HydrogelFilm</v-list-item-title>
            </v-list-item-content>
          </v-list-group>
          <v-list-item>
            <v-list-item-title>PRICE</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>ACCESS</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>DISCLAIMER</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

  </header>
</template>

<script>
export default{
  data() {
    return{
      drawer: false,
    }
  }
}
</script>