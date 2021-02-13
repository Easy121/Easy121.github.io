<template>
	<div id="hello">
		{{ msg }}
	</div>
</template>

<script>
export default {
	el: '#hello',
	data: () => {
		return {
			msg: "Hello World"
		}
	}
}
</script>

<style>

</style>