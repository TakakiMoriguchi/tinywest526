<template>
  <main class="form">
    <v-container
      class="jumboTron-price d-flex align-end mb-10"
      fluid
    >
      <v-container class="about-title">
        <h1>料金</h1>
        <p>Price</p>
      </v-container>
    </v-container>

    <section class="row d-flex justify-center priceTable mb-5">
    <v-form ref="form">
      <v-text-field
        v-model="model"
        :counter="max"
        :rules="rules"
        label="First name"
      ></v-text-field>
    </v-form>
    </section>
    <global-footer />
  </main>
</template>

<script>
</script>