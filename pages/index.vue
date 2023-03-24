<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <main>
    <v-container
      class="jumboTron-index"
      fluid
    >
      <v-container class="text-center" fill-height>
        <div class="mx-auto">
          <h2>芦屋の小規模スマホ修理店</h2>
          <h5>予約制（in work and place）</h5>

          <v-btn color="deep-purple lighten-2 mt-2" depressed>
            <a href="tel:07043192480">今すぐ電話する！</a>
          </v-btn>
        </div>
      </v-container>
    </v-container>

    <section class="container">
      <index-about />
      <index-blog />
      <index-price />
      <index-map />
    </section>

    <global-footer />
  </main>
</template>
