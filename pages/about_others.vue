<template>
  <main class="about_page">
    <v-container
      class="jumboTron-others d-flex align-end mb-10"
      fluid
    >
      <v-container class="about-title">
        <h1>ハイドロゲルフィルム・その他修理</h1>
        <p>HydrogelFilm / Others</p>
      </v-container>
    </v-container>

    <section class="container about_description pa-5">
      <v-row>
        <v-col cols=12 lg=8 md=8 sm=8 xs=12>
          <h4><v-icon>mdi-tools</v-icon>&nbsp;ハイドロゲルフィルム</h4>
          <p>
            当店で取り扱うハイドロゲルフィルムは、どんな衝撃も耐えれるわけではありませんが、耐衝撃性が高く、また多少の傷（へこみ）であれば自己再生します。<br />
            仕上がりは全面コーティングされたようで、滑りもよく、リピーターの方も多数いらっしゃいます。<br />
            貼り付けに技術が必要で、ほぼ当店限定でしか手に入れることが出来ないでしょう。
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;強化ガラス</h4>
          <p>
            強化ガラスは高度がカッターの刃と同等の硬さを持ち、傷に強い特徴があります。<br />
            ガラス面は強い衝撃が加わるか、小さな傷が積み重なって割れてしまうことが多いので、擦り傷のつきやすい環境であれば強化ガラスをオススメします。
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;カメラ</h4>
          <p>
            iphone8/SE2、iphone11pro/promaxはアウトカメラが衝撃に弱く、カタカタと無限フォーカスしたり、ブラックアウトやホワイトアウトする症状がよく見られます。<br />
            またカメラの表面ガラスが割れてしまうケースも多く見てきました。<br />
            カメラは高額なので、なるべく安く修理できるようにパーツを仕入れていますが、それぞれ数千円単位で値段が違うため、時価となります。何卒ご了承くださいませ。
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;その他パーツ</h4>
          <p>
            インカメラ・バイブレーター、スピーカー、コネクタ部分の交換などの修理も承っています。<br />
            androidパーツも物によっては手に入る場合がありますので、お気軽にお問い合わせください。
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;背面ガラス割れ</h4>
          <p>
            iphone8以降はワイアレス充電に対応するため、背面がガラスに変更されましたが、これによって背面のガラスが割れてしまうケースも多く存在します。<br />
            この場合フレームごと交換になりますので、色や程度のご指定を承ることが出来ない場合があります。<br />
            しかし、背面の色と元のボタンの色を組み合わせてオリジナリティを出すことも出来ますので、お気軽にご相談ください。           
          </p>

          <h4><v-icon>mdi-tools</v-icon>&nbsp;水没</h4>
          <p>
            iphoneもandroidも過剰広告によりあたかも水没しないような製品というプロモーションがされていますが、状況によって簡単に水没します。<br />
            もし水没してしまった場合は概ね８時間以内にお持ち込み頂ければ修理することが出来るかもしれません。<br />
            水没の程度によって他のパーツが壊れてしまっていますが、早急に対応することによりデータの喪失を免れることが出来ます。
          </p>

        </v-col>

        <v-col cols=12 lg=4 md=4 sm=4 xs=0>
          <v-img src="/images/about_others_sub1.jpg" />
          <v-img src="/images/about_others_sub2.jpg" />
          <v-img src="/images/about_others_sub3.jpg" />
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
