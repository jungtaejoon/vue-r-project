<template>
  <div>
    <paragraph-history
      v-for="output in makingSize"
      :id="output"
      :key="output"
    ></paragraph-history>
  </div>
</template>

<script>
  import ParagraphHistory from './ParagraphHistory'
  export default {
    name: "paragraph-history-factory",
    props: {
      makingSize: {
        type: Number,
        default() {
          return 1
        }
      }
    },
    data() {
      return {
        nextParagraphHistoryId: 0,
        outputs: []
      }
    },
    components: {
      ParagraphHistory
    },
    methods: {
      getParagraphHistories(size) {
        for(let i = 0; i < size; i++) {
          this.outputs.push(this.nextParagraphHistoryId++);
        }
      }
    }
  }
</script>

<style scoped>

</style>
