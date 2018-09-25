<template>
  <div>
    <input autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
    <SearchIcon class="searchButton" @click="search($event)"/>
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

div {
  margin: 20px 20px;
  display: flex;
  justify-content: center;
}

input {
  border: none;
  border-bottom: 2px solid #9d8189;
  outline: none;
  color: #9d8189;
}

.searchButton {
  cursor: pointer;
  color: #9d8189;
}

.searchButton:hover {
  color: #f4acb7;
}

.searchButton:active {
  transform: translateY(4px);
}
</style>
