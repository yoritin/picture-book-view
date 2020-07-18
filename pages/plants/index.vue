<template>
  <div>
    <div v-for="plant in plants" :key="plant.id">
      <Plant />
    </div>
  </div>
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
        },
        {
          id: 2,
          name: 'Tillandsia ionantha fuego',
          purchase_date: '2020-02-02',
        },
        {
          id: 3,
          name: 'Tillandsia ionantha fuego',
          purchase_date: '2020-02-02',
        },
      ],
    }
  },
}
</script>
