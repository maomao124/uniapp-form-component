<template>
	<view>
		<picker mode="selector" :range="data" @change="change" @cancel="cancel()">点击普通选择器</picker>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				data:['1','2','3','4','5'],
			}
		},
		methods: {
			change(e)
			{
				console.log("值被改变了，索引：",e.target.value,"值：",this.data[e.target.value]);
			},
			cancel()
			{
				console.log("取消");
			}
		}
	}
</script>

<style>

</style>
