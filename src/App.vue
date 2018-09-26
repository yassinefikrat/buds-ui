<template>
  <div id="app">
    <ChuccButton @click="processClickOnNew">New</ChuccButton>
    <ChuccIconButton @click="processClickOnSettings"><SettingsIcon/></ChuccIconButton>
    <ChuccTag @click="processClickOnIdTag">157-361</ChuccTag>
    <ChuccNormalText>Normal Text</ChuccNormalText>
    <ChuccSearchBar @search="processClickOnSearch"/>
  </div>
</template>

<script>
import { SettingsIcon } from 'vue-feather-icons'
import HelloWorld from './components/HelloWorld'
import ChuccButton from './components/ChuccButton'
import ChuccIconButton from './components/ChuccIconButton'
import ChuccTag from './components/ChuccTag'
import ChuccNormalText from './components/ChuccNormalText'
import ChuccSearchBar from './components/ChuccSearchBar'

export default {
  name: 'App',
  components: {
    SettingsIcon,
    HelloWorld,
    ChuccButton,
    ChuccIconButton,
    ChuccTag,
    ChuccNormalText,
    ChuccSearchBar
  },
  methods: {
    processClickOnNew: function() {
      alert('Clicked on New')
    },
    processClickOnSettings: function() {
      alert('Clicked on Settings')
    },
    processClickOnIdTag: function() {
      alert('Clicked on Id Tag')
    },
    processClickOnSearch: function(term) {
      alert('Clicked on Search with term ' + term)
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
