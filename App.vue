<template>
  <h1 @click="handleClick">hi there!</h1>
</template>

<script>
	export default {
		mounted () {
			var vConsole = new VConsole()
			vConsole.setOption('maxLogNumber', 5000)
			vConsole.log('Hello world')
		},
		methods: {
			handleClick (e) {
				alert(e)
			}
		}
	}
</script>