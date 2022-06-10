<template>
	<view class="box">
		<th-autograph 
		:is-download="false" 
		@submit="getFile" 
		canvas-id="autograph">
		</th-autograph>
	</view>
</template>

<script>
	import thAutograph from "../../components/th-autograph/th-autograph.vue"
	export default {
		components:{
			thAutograph
		},
		methods:{
			getFile(path){
				console.log(path)
			}
		}
	}
</script>

<style>
	page{
		width: 100%;
		height: 100%;
	}
	.box{
		width: 100%;
		height: 100%;
	}
</style>
