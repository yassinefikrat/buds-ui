<template>
  <div id="app">
    <ChuccButton label="New"/>
    <ChuccIconButton><AirplayIcon/></ChuccIconButton>
  </div>
</template>

<script>
import { AirplayIcon } from 'vue-feather-icons'
import HelloWorld from './components/HelloWorld'
import ChuccButton from './components/ChuccButton'
import ChuccIconButton from './components/ChuccIconButton'

export default {
  name: 'App',
  components: {
    AirplayIcon,
    HelloWorld,
    ChuccButton,
    ChuccIconButton
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
