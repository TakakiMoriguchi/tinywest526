<template>
  <main class="about_page">
    <v-container
      class="jumboTron-battery d-flex align-end mb-10"
      fluid
    >
      <v-container class="about-title">
        <h1>バッテリー交換</h1>
        <p>iphone / android battery replacement</p>
      </v-container>
    </v-container>

    <section class="container about_description pa-5">
      <v-row>
        <v-col cols=12 lg=8 md=8 sm=8 xs=12>
          <h4><v-icon>mdi-tools</v-icon>&nbsp;中国製バッテリーは安全？</h4>
          <p>
            iphoneが出た当初、中国でバッテリーが発火するという事件がありましたが、果たして中国製バッテリーは安全なのでしょうか？<br />
            そもそもiphoneもandroidも中国がメインの製造を承っており、純日本製のバッテリーというものはありません。<br />
            その代わり、当店ではＰＳＥ認証という審査をクリアしたものを仕入れて使用しています。
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;バッテリー交換の目安</h4>
          <p>
            設定からバッテリーの総残量を確認することが出来ます。<br />
            おおよそ80%～90%が交換目安（昼過ぎには充電が無くなる程度）になります。<br />
            またリチウムイオンは純正・非純正問わず、稀に大きく膨らんでしまうことがあります。<br />
            バッテリーが膨らむと画面が浮き、最終的には画面が破損してしまいます。<br />
            隙間が見受けられる場合は早急にお申し付けください。
          </p>
          
          <h4><v-icon>mdi-tools</v-icon>&nbsp;androidのバッテリー交換について</h4>
          <p>
            android製品は修理できるものが限られますので一度お問い合わせ下さい。
          </p>
        </v-col>

        <v-col cols=12 lg=4 md=4 sm=4 xs=0>
          <v-img src="/images/about_battery_sub1.jpg" />
          <v-img src="/images/about_battery_sub2.jpg" />
          <v-img src="/images/about_battery_sub3.jpg" />
        </v-col>
      </v-row>
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
