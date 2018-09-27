<template>
  <div class="container">
    <span class="title">{{title}}</span>
    <div>
      <ChuccTag v-for="tag in tags" :key="tag">{{tag}}</ChuccTag>
    </div>
  </div>
</template>

<script>
import ChuccTag from "./ChuccTag";
export default {
  name: "ChuccTableItem",
  components: {
    ChuccTag
  },
  props: {
    title: {
      type: String,
      required: true
    },
    tags: {
      type: Array,
      required: false
    }
  }
};
</script>

<style scoped>
* {
  font-family: "Hack", monospace;
}

.container {
  display: flex;
  justify-content: space-between;
  background-color: #9D8189;
  margin: 10px 10px;
  padding: 4px 5px 5px 10px;
  border-radius: 5px;
}

.title {
  margin-top: 2px;
  color: #FFE5D9;
}
</style>
