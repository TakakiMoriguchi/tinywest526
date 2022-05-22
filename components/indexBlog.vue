<template>
  <div>
    <div class="sub_contents_title" id="index_latest">
      LATEST
    </div>

    <v-row class="blog">
      <!-- {{ cardData }} -->
      <v-col
        v-for="val in cardData"
        :key="val.id"
        cols="12" md="4" xs="10"
      >
        <v-card outlined tile dark>
          <v-card-title class="blog-title">{{ val.title }}</v-card-title>
          <div class="blog-category">
            <v-chip small>{{ val.category[0] }}</v-chip>
          </div>
          <v-card-text class="blog-text">
            <v-icon small class="mb-1">mdi-pencil-box-outline</v-icon>&nbsp;{{ dayFormat(val.publishedAt) }}
            <p>{{ textFormat(val.content) }}</p>
          </v-card-text>
          <v-card-actions>
            <NuxtLink :to="'latest/' + val.id" class="card-link">Read More...</NuxtLink>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>

  </div>
</template>

<script>
import axios from 'axios'

export default {

  data(){
    return {
      responseData: ''
    }
  },

  mounted() {
    axios.get('https://tinywest.microcms.io/api/v1/blog/', {headers: { 'X-MICROCMS-API-KEY': '36d4ea8b9b334e57837240c45e614e9fce6b' }}).then(response => (
      this.responseData = response.data.contents
    ))
  },

  computed: {
    cardData() {
      return this.responseData.slice(0,3)
    },

    textFormat () {
      return (arg) => {
        return arg.replace(/<("[^"]*"|'[^']*'|[^'">])*>/g,'').substr(0, 150).concat('...')
      }
    },

    dayFormat () {
      return (arg) => {
        return arg.substr(0, 10)
      }
    }
  }
}
</script>