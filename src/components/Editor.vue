<template>
  <div>
    <paragraph-history-factory
      :makingSize="size"
    ></paragraph-history-factory>
  </div>
</template>

<script>
  import ParagraphHistoryFactory from './ParagraphHistoryFactory'

  export default {
    name: "Editor",
    components: {
      ParagraphHistoryFactory
    },
    data() {
      return {
        size: 6
      }
    },
    created() {

    }
  }
</script>

<style scoped>

</style>
