<template>
  <div>
    <div class="sub_contents_title">
      ABOUT
    </div>

    <v-row class="about_wrapper">
      <v-col cols="12" md="4" xs="10">
        <v-card outlined dark class="card-style">
          <v-img
            src="/images/about_display.jpg"
            height="572px"
            width="100%"
            class="d-flex align-end"
          >
            <div class="card-content">
              <v-card-title>Display</v-card-title>
              <v-card-subtitle>Good Quality LCD/OLED Screen</v-card-subtitle>
              <v-card-text>
                最高品質のLCD/OLEDパネルを入荷し、発色、タッチ感も純正同等に良好です。また工場では何度もテストを重ねることによって動作の保証がされており、安心してお使い頂けます。
              </v-card-text>
              <v-card-actions class="d-flex align-right">
                <NuxtLink to="about_display" class="card-link">
                  LearnMore&nbsp;<v-icon small>mdi-arrow-right</v-icon>
                  <hr />
                </NuxtLink>
              </v-card-actions>
            </div>
          </v-img>
        </v-card>
      </v-col>
      <v-col cols="12" md="4" xs="10">
        <v-card outlined dark class="card-style">
          <v-img
            src="/images/about_battery.jpg"
            height="572px"
            width="100%"
            class="d-flex align-end"
          >
            <div class="card-content">
              <v-card-title>Battery</v-card-title>
              <v-card-subtitle>All Battery Passed PSE Rules</v-card-subtitle>
              <v-card-text>
                全て電気用品安全法（PSE）に合格したパーツで、ゲームや動画編集などを行うスマホヘビーユーザーには希望により大容量バッテリーも準備することができます。
              </v-card-text>
              <v-card-actions class="d-flex align-right">
                <NuxtLink to="#" class="card-link">
                  LearnMore&nbsp;<v-icon small>mdi-arrow-right</v-icon>
                  <hr />
                </NuxtLink>
              </v-card-actions>
            </div>
          </v-img>
        </v-card>
      </v-col>
      <v-col cols="12" md="4" xs="10">
        <v-card outlined dark class="card-style">
          <v-img
            src="/images/about_hydrogel.jpg"
            height="572px"
            width="100%"
            class="d-flex align-end"
          >
            <div class="card-content">
              <v-card-title>Hydrogel Film</v-card-title>
              <v-card-subtitle>Best Choice Screen Protection</v-card-subtitle>
              <v-card-text>保護フィルムはガラス製・ペット製など様々な素材がある中、飛びぬけて衝撃に強いのがハイドロゲルフィルム。硬さで保護するのではなく、柔らかさで保護します。</v-card-text>
              <v-card-actions class="d-flex align-right">
                <NuxtLink to="#" class="card-link">
                  LearnMore&nbsp;<v-icon small>mdi-arrow-right</v-icon>
                  <hr />
                </NuxtLink>
              </v-card-actions>
            </div>
          </v-img>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>