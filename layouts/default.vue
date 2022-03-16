<template>
  <v-app>
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
