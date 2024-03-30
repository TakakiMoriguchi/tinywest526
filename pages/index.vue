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

          <div style="color: red; background-color: white; font-weight: bold">
            3月末をもって閉店いたしました。<br />
            ご愛顧いただき、誠にありがとうございました。<br />
          </div>
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
