<template>
  <main class="about_page">
    <v-container
      class="jumboTron-display d-flex align-end mb-10"
      fluid
    >
      <v-container class="about-title">
        <h1>画面修理</h1>
        <p>iphone / android display replacement</p>
      </v-container>
    </v-container>

    <section class="container display_description pa-5">
      <v-row>
        <v-col cols=12 lg=8 md=8 sm=8 xs=12>
          <h4><v-icon>mdi-tools</v-icon>&nbsp;意外にも"旬"があるiphoneパーツ</h4>
          <p>
            当店が知っている限り、中国のOEMメーカーは７社以上、さらにクオリティも合わせると１つの画面だけで３０種類以上あるかもしれません。<br />
            さらにそれぞれのメーカーで、時期やロットにより良し悪しがあり、それらを見極めて良いパーツを仕入れるのはかなりの技術とコネクションを要します。<br />
            当店では信頼できるパーツショップと密に連絡を取り、その時々で良いものを選定して仕入れています。
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;iphone画面の種類</h4>
          <p>
            iphoneの画面は大きく分けて３種類ございます。<br /><br />

            ・規格品<br />
            こちらは所謂コピーパネルです。<br />
            主に激安修理店で採用されており、７層構造になっているため純正パネルよりも分厚くなりますが、リーズナブルに修理することが出来ます。<br />
            当店では7plus以前の製品に採用していますが、要望により上のランクのincell品を仕入れて修理することも可能です。<br />
            →&nbsp;古い製品を安く修理したい方にオススメします。<br /><br />

            ・incell品<br />
            スーパーコピーといわれる製品で、純正と同じ５層構造で製造されているため、画面浮きがありません。<br />
            規格品と比べると高値ではありますが、発色やガラス、コネクタの強度などが違います。<br />
            当店では8以降の製品に採用していますが、要望により下のランクの規格品で安くお見積り出来ます。<br />
            →&nbsp;今後も長く使い方にオススメします。<br /><br />

            ・再生品<br />
            割れたガラスのみを工場にて交換した純正液晶×高純度ガラスの製品です。<br />
            非正規で手に入る最上のパーツで、純正の液晶を使用していますので、発色良好です。<br />
            当店では<strong>事前予約</strong>にて修理することが可能です。<br />
            →&nbsp;純正に近い製品で修理されたい方にオススメします。<br />
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;なぜincell品を採用しているのか</h4>
          <p>
            当店では、古い製品は修理価格の相場が落ちますのでやむなく規格品を使用していますが、基本的にはincell品を使用しています。<br />
            なぜなら明らかに発色・強度・画面の厚みが違うからです。<br />
            毎日何時間も使うものですし、多少値段は上がりますが、incell品を採用しています。<br />
          </p>
          
          <h4><v-icon>mdi-tools</v-icon>&nbsp;androidのガラス割れについて</h4>
          <p>
            android製品はパーツの流通が乏しく、画面修理が出来るものは多くありません。<br />
            修理できる製品に関しては随時料金表に乗せるようにしていますが、一度お問い合わせ下さい。<br />
            とはいえ、ある程度ブランドごとに修理できるか出来ないかが決まっていますので以下をご参考ください。
          </p>
          <table>
            <tr>
              <th>AQUOS</th>
              <td>×</td>
              <td>修理出来ない</td>
            </tr>
            <tr>
              <th>Xperia</th>
              <td>△</td>
              <td>古い機種に限り修理出来る。</td>
            </tr>
            <tr>
              <th>Galaxy</th>
              <td>△</td>
              <td>A系は修理出来ず、S系は修理出来るが非常に高額になる</td>
            </tr>
            <tr>
              <th>OPPO</th>
              <td>×</td>
              <td>修理出来ない</td>
            </tr>
            <tr>
              <th>GooglePixel</th>
              <td>△</td>
              <td>修理出来るものがかなり限られる</td>
            </tr>
            <tr>
              <th>Xiaomi</th>
              <td>△</td>
              <td>修理出来るが、時間がかかる</td>
            </tr>
          </table>
        </v-col>

        <v-col cols=12 lg=4 md=4 sm=4 xs=0>
          <v-img src="/images/about_display_sub1.jpg" />
          <v-img src="/images/about_display_sub2.jpg" />
          <v-img src="/images/about_display_sub3.jpg" />
          <v-img src="/images/about_display_sub4.jpg" />
          <v-img src="/images/about_display_sub5.jpg" />
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
