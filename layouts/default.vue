<template>
  <v-app class="w-100">
    <appBar />
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
import appBar from '~/components/appBar'

export default {
  components: {
    appBar
  }
}
</script>
