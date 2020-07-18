<template>
  <v-container>
    <v-row>
      <v-col v-for="plant in plants" :key="plant.id" md="4" sm="12">
        <Plant :plant="plant" />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Plant from '~/components/Plant.vue'

export default {
  components: {
    Plant,
  },

  data() {
    return {
      plants: [
        {
          id: 1,
          name: 'Tillandsia ionantha rubra',
          purchase_date: '2020-02-02',
          content: 'aaaa',
        },
        {
          id: 2,
          name: 'Tillandsia ionantha fuego',
          purchase_date: '2020-02-02',
          content: 'bbbb',
        },
        {
          id: 3,
          name: 'Tillandsia ionantha pp',
          purchase_date: '2020-02-02',
          content: 'cccc',
        },
      ],
    }
  },
}
</script>
