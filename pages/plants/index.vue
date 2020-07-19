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
          image:
            'https://pbs.twimg.com/media/EYoAbcqVAAI8Kc1?format=jpg&name=large',
          content: 'でかいイオナンタ',
        },
        {
          id: 2,
          name: 'Tillandsia ionantha fuego',
          purchase_date: '2020-02-02',
          image:
            'https://pbs.twimg.com/media/EcEKhdqUEAAGlUZ?format=jpg&name=large',
          content: 'タイの業者から購入したイオナンタ、かわいい',
        },
        {
          id: 3,
          name: 'Tillandsia ionantha pp',
          purchase_date: '2020-02-02',
          image:
            'https://pbs.twimg.com/media/EYeB9EZUcAAy4CG?format=jpg&name=large',
          content: 'ちら庭で買ったイオナンタ、かわいい',
        },
        {
          id: 3,
          name: 'Tillandsia ionantha pp',
          purchase_date: '2020-02-02',
          image:
            'https://pbs.twimg.com/media/EYTjyvXXkAAbNoc?format=jpg&name=large',
          content: 'ちら庭で買ったイオナンタ、かわいい',
        },
        {
          id: 3,
          name: 'Tillandsia ionantha pp',
          purchase_date: '2020-02-02',
          image:
            'https://pbs.twimg.com/media/Eb_QjXzUcAElXJV?format=jpg&name=large',
          content: 'ちら庭で買ったイオナンタ、かわいい',
        },
        {
          id: 3,
          name: 'Tillandsia ionantha pp',
          purchase_date: '2020-02-02',
          image:
            'https://pbs.twimg.com/media/EXXWgyhVAAELf0Z?format=jpg&name=large',
          content: 'ちら庭で買ったイオナンタ、かわいい',
        },
      ],
    }
  },
}
</script>
