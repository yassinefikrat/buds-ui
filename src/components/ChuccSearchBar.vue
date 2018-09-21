<template>
  <div>
    <input/>
    <div class="searchButton"><SearchIcon @click="search($event)"/></div>
  </div>
</template>

<script>
import { SearchIcon } from 'vue-feather-icons'
export default {
  name: 'ChuccSearchBar',
  components:{
    SearchIcon
  },
  methods: {
    search: function(e) {
      this.$emit('search', e)
    }
  }
}
</script>

<style scoped>
* {
  font-family: 'Hack', monospace;
}

input {
  border: none;
  border-bottom: 2px solid #9d8189;
  outline: none;
}

.searchButton {
  cursor: pointer;
  color: #9d8189;
  padding: 10px 10px;
  display: inline-block;
}

.searchButton:hover {
  color: #f4acb7;
}

.searchButton:active {
  transform: translateY(4px);
}
</style>
