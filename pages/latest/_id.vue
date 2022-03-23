<template>
  <v-container>
    <div class="blog-contents">
      <div class="blog-title">
        <h2>{{ blogData.title }}</h2>
        <span class="blog-subtitle">{{ blogData.category[0] }}：{{ blogData.createdAt }}</span>
      </div>

      <p v-html="blogData.content"></p>
    </div>
  </v-container>
</template>

<script>
import axios from 'axios'

export default{
  data(){
    return {
      res: '',
      blogData: {
        createdAt: '',
        title: '',
        content: '',
        category: ''
      }
    }
  },

  created() {
    let params = this.$route.params.id || ''
    axios.get('https://tinywest.microcms.io/api/v1/blog/' + params, {headers: { 'X-MICROCMS-API-KEY': '36d4ea8b9b334e57837240c45e614e9fce6b' }}).then(response => {
      this.res = response.data,
      this.blogData.createdAt = response.data.createdAt,
      this.blogData.title = response.data.title,
      this.blogData.content = response.data.content,
      this.blogData.category = response.data.category
    })
  },

}


</script>