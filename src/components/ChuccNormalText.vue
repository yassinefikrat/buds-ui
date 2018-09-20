<template>
  <span>
    <slot></slot>
  </span>
</template>

<script>
export default {
  name: 'ChuccNormalText'
}
</script>

<style scoped>
* {
  font-family: 'Hack', monospace;
}

span {
  color: #9d8189;
  display: inline-block;
  font-size: 14px;
}
</style>
