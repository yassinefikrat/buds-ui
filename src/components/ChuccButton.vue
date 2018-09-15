<template>
  <button @click="click($event)">
    {{ label }}
  </button>
</template>

<script>
export default {
  name: 'ChuccButton',
  props: {
    label: {
      type: String,
      required: true
    }
  },
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

button {
  cursor: pointer;
  background-color: #ffcad4;
  border: none;
  border-radius: 5px;
  color: #9d8189;
  padding: 10px 40px;
  display: inline-block;
  font-size: 18px;
  box-shadow: 0 9px #9d8189;
  outline: none;
}

button:hover {
  background-color: #f4acb7;
}

button:active {
  background-color: #f4acb7;
  box-shadow: 0 5px #9d8189;
  transform: translateY(4px);
}
</style>
