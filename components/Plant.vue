<template>
  <v-card class="mb-4" :to="`/plants/${plant.id}`">
    <v-card-title>{{ plant.name }}</v-card-title>
    <v-img :src="plant.image" height="200px"></v-img>
    <v-card-subtitle>{{ plant.purchase_date }}</v-card-subtitle>
    <v-card-text>{{ plant.content }}</v-card-text>
  </v-card>
</template>

<script>
export default {
  props: {
    plant: {
      type: Object,
      required: true,
    },
  },
}
</script>
