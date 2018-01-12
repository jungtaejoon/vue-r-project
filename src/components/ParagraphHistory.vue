<template>
  <div>
    {{id}}
  </div>
</template>

<script>
  export default {
    props: {
      id: {
        type: Number,
        default() {
          return 0
        }
      }
    },
    name: "paragraph-history"
  }
</script>

<style scoped>

</style>
