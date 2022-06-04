<template>
  <header class="appBar">
    <v-app-bar
      app
      dark
    >
      <v-toolbar-title>
        <nuxt-link to="/" class="siteTitle">
          <img
            src="/images/logo.svg"
            alt="tinywest_logo"
          />
          <h1>tinyWEST</h1>
        </nuxt-link>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon
        @click="drawer=true"
        name="navbar"
      ></v-app-bar-nav-icon>
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
        <div
          @click="drawer=false"
          class="closeButton"
        >
          <span class="batsu"></span>
        </div>

        <v-list-item-group>
          <v-list-item>
            <v-list-item-title>
              <nuxt-link to="/#index_latest">NEWS</nuxt-link>
            </v-list-item-title>
          </v-list-item>
          <v-list-group>
            <template v-slot:activator>
              <v-list-item-title>ABOUT</v-list-item-title>
            </template>
            <v-list-item-content>
              <v-list-item-title class="aboutChild">
                <nuxt-link to="about_display">DISPLAY</nuxt-link>
              </v-list-item-title>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-title class="aboutChild">
                <nuxt-link to="about_battery">BATTERY</nuxt-link>
              </v-list-item-title>
            </v-list-item-content>
            <v-list-item-content>
              <v-list-item-title class="aboutChild">
                <nuxt-link to="about_others">HydrogelFilm / Others</nuxt-link>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-group>
          <v-list-item>
            <v-list-item-title>
              <nuxt-link to="price">PRICE</nuxt-link>
            </v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>
              <nuxt-link to="/#index_access">ACCESS</nuxt-link>
            </v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>
              <nuxt-link to="/latest/5l_j01l87xn">DISCLAIMER</nuxt-link>
            </v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>
              <nuxt-link to="/form">FORM</nuxt-link>
            </v-list-item-title>
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