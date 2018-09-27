<template>
  <div>
    <input type="text" v-model="searchTerm" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
    <SearchIcon class="searchButton" @click="search(searchTerm)"/>
  </div>
</template>

<script>
import { SearchIcon } from "vue-feather-icons";
export default {
  name: "ChuccSearchBar",
  components: {
    SearchIcon
  },
  data: () => {
      return {
        searchTerm: ''
      }
  },
  methods: {
    search: function(st) {
      this.$emit("search", st);
    }
  }
};
</script>

<style scoped>
* {
  font-family: "Hack", monospace;
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
  background-color: #FFE5D9;
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
