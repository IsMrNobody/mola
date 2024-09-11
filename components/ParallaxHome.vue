<template>
  <v-parallax
    contain
    height="300"
    src="https://res.cloudinary.com/dku13l2ep/image/upload/v1725981476/JARTATE/Ciudad/caracas/Mola/banner6_yrvds2.png"
  >
    <v-col class="text-center">
      <v-img width="180" class="mx-auto mt-12" :src="merchant.logo"> </v-img>
      <h2>{{ merchant.slogan }}</h2>
      <h3>Ahora puedes pedir tu delivery cuando quieras!</h3>
    </v-col>
  </v-parallax>
</template>

<script>
export default {
  computed: {
    merchant() {
      return this.$store.state.merchant
    },
  },
}
</script>

<style scoped></style>
