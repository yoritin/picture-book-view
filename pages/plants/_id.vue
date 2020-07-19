<template>
  <div>
    <h1>detail page</h1>
    <p>page_id:{{ page_id }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      page_id: [],
    }
  },

  created() {
    this.page_id = this.$route.params.id
  },
}
</script>
