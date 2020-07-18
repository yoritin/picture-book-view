<template>
  <v-card class="mb-4">
    <v-card-title>
      <p>{{ plant.name }}</p>
      <p>{{ plant.purchase_date }}</p>
    </v-card-title>
    <v-card-text>Plant info</v-card-text>
  </v-card>
</template>

<script>
export default {
  props: ['plant'],
  created() {
    console.log(this.plant)
  },
}
</script>
