<template>
  <main>
    <v-container
      class="jumboTron-index"
      fluid
    >
      <v-container class="text-center" fill-height>
        <div class="mx-auto">
          <h2>データそのまま！<br />最短30分で即日修理。</h2>
          <h5>予約制（in work and place）</h5>

           <!--
          <v-btn color="deep-purple lighten-2 mt-2" depressed>
            <a href="tel:07043192480">今すぐ電話する！</a>
          </v-btn>
          -->

          <h1 class="my-2 red">休業中</h1>
          <span>11月上旬再開予定</span>
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
