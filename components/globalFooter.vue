<template>
  <v-footer dark padless>
    <v-card
      flat
      tile
      class="white--text text-center"
      style="width: 100% !important;"
    >
      <v-card-text>
        <v-btn class="mx-4 white--text" href="https://www.instagram.com/tinywest526/" target="_blank" icon>
          <v-icon size="24px">mdi-instagram</v-icon>
        </v-btn>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>tinyWEST</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>