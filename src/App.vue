<template>
  <div id="app">
    <ChuccButton @click="processClickOnNew">New</ChuccButton>
    <ChuccIconButton @click="processClickOnSettings"><SettingsIcon/></ChuccIconButton>
    <ChuccTag @click="processClickOnIdTag">157-361</ChuccTag>
  </div>
</template>

<script>
import { SettingsIcon } from 'vue-feather-icons'
import HelloWorld from './components/HelloWorld'
import ChuccButton from './components/ChuccButton'
import ChuccIconButton from './components/ChuccIconButton'
import ChuccTag from './components/ChuccTag'

export default {
  name: 'App',
  components: {
    SettingsIcon,
    HelloWorld,
    ChuccButton,
    ChuccIconButton,
    ChuccTag
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
