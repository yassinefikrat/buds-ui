<template>
  <span @click="click($event)">
    <strong><slot></slot></strong>
  </span>
</template>

<script>
export default {
  name: 'ChuccTag',
  methods: {
    click: function(e) {
      this.$emit('click', e)
    }
  }
}
</script>

<style scoped>
* {
  font-family: 'Hack', monospace;
}

span {
  cursor: pointer;
  background-color: #ffcad4;
  border: none;
  border-radius: 5px;
  color: #9d8189;
  padding: 2px 5px;
  margin-left: 5px;
  display: inline-block;
  font-size: 12px;
}

span:hover {
  background-color: #f4acb7;
}
</style>
