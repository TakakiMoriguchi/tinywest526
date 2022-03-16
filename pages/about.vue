<template>
  <div class="scrollSnap">
    <v-container class="area">
      Display
    </v-container>
    <v-container class="area">
      Battery
    </v-container>
    <v-container class="area">
      Hydrogel Film
    </v-container>
  </div>
</template>

<script>

export default {
}
</script>

<style>
  .scrollSnap {
    overflow: auto;
    scroll-snap-type: y mandatory;
    height: 100vh;
  }

  .area {
    scroll-snap-align: start;
    height: 100vh;
  }
</style>