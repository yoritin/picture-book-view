<template>
  <div>
    <Plant />
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
          name: 'Tillandsia ionantha',
          purchase_date: '2020-02-02',
        },
      ],
    }
  },
}
</script>
