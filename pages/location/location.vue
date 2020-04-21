<template>
	<view>
		
		<text>hello world</text>
		<map  longitude="130.1321" latitude="39.12311"></map>
		<button @click="tapName">click Me!</button>
		
	</view>
</template>


<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			tapName: function(){
				alert("hello world!")
			}
		}
	}
</script>

<style>

</style>
