<template>

  <button class="btn-chucc">
		<slot></slot>
  </button>

</template>

<script>

	export default {
	  name: 'ChuccIconButton'
	}

</script>

<style scoped>

  * {
    font-family: 'Hack', monospace;
  }

  button {
    cursor: pointer;
    background-color: #FFCAD4;
    border: none;
    border-radius: 5px;
    color: #9D8189;
    padding: 10px 15px;
    display: inline-block;
    font-size: 16px;
    box-shadow: 0 9px #9D8189;
    outline: none;
  }

  button:hover {
    background-color: #F4ACB7;
  }

  button:active {
    background-color: #F4ACB7;
    box-shadow: 0 5px #9D8189;
    transform: translateY(4px);
  }

</style>
