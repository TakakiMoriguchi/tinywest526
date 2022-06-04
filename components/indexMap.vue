<template>
  <div>
    <div id="index_access" class="sub_contents_title">
      MAP
    </div>

    <div class="d-flex justify-center">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d9684.636940938244!2d135.30219875047837!3d34.7337099010154!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6000f3a7208372d3%3A0x55f15d0bee38f932!2zdGlueVdFU1ToiqblsYsgLSDjgrnjg57jg5vjg7tpcGhvbmXkv67nkIblupc!5e0!3m2!1sja!2sjp!4v1646920920074!5m2!1sja!2sjp"
        width="600"
        height="450"
        style="border:0;"
        allowfullscreen=""
        loading="lazy"
      />
    </div>

    <div class="text-center pa-4">
      <h6 class="text-h6">
        営業時間：11:00 ～ 17:30<span class="subtitle-2">【予約制】</span>
      </h6>

      <p>
        〒659-0093&nbsp;​芦屋市船戸町5-26 マリアキャリーヌビル2F<br>
      </p>

      <p>
        <nuxt-link to="tel:0797249062">
          <v-icon small>mdi-phone-classic</v-icon>&nbsp;{{ telNumber }}<br>
        </nuxt-link>
      </p>
      <p>
        <nuxt-link to="/form">
          <v-icon small>mdi-format-list-text</v-icon>&nbsp;お問合せ
        </nuxt-link>
      </p>

      <p class="text-body-2 pa-3">
        JR芦屋駅：北に徒歩３分、阪急芦屋川駅：東南東に徒歩7分<br>
        入口の扉が閉まっている場合はインターホンを鳴らしてください($・・)/o
      </p>
    </div>

  </div>
</template>

<script>
export default {
  data () {
    return {
      telNumber: '0797-24-9062'
    }
  }
}
</script>
