<template>
  <main>
    <v-container
      class="jumboTron"
      fluid
    >
      <v-container class="text-center" fill-height>
        <div class="mx-auto">
          <h2>データそのまま！<br />最短30分で即日修理。</h2>
          <h5>予約制（in work and place）</h5>
          <v-btn color="deep-purple lighten-2 mt-2" depressed>今すぐ電話する！</v-btn>
        </div>
      </v-container>
    </v-container>

    <section class="container">
      <index-about />
      <index-blog />
      <index-price />
      <index-map />
    </section>


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
  </main>
</template>
