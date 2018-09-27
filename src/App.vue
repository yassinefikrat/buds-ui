<template>
  <div id="app">
    <ChuccButton @click="processClickOnNew">New</ChuccButton>
    <ChuccIconButton @click="processClickOnSettings"><SettingsIcon/></ChuccIconButton>
    <ChuccTag @click="processClickOnIdTag">157-361</ChuccTag>
    <ChuccNormalText>Normal Text</ChuccNormalText>
    <ChuccSearchBar @search="processClickOnSearch"/>
    <ChuccTableItem title="Test connexion from a server to a DB" v-bind:tags="tags"/>
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
import ChuccTableItem from './components/ChuccTableItem'

export default {
  name: 'App',
  components: {
    SettingsIcon,
    HelloWorld,
    ChuccButton,
    ChuccIconButton,
    ChuccTag,
    ChuccNormalText,
    ChuccSearchBar,
    ChuccTableItem
  },
  data() {
    return {
      tags: ['178-772', '129-037']
    }
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
