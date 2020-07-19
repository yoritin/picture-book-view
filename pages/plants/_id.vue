<template>
  <h1>detail page</h1>
</template>

<script>
export default {
  created() {
    console.log(this.$route.params.id)
  },
}
</script>
