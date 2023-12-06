<template>
	<view>
		<picker mode="date" @change="change" start="2023-06-03" 
		end="2024-07-22" @cancel="cancel()">点击日期选择器</picker>
	</view>
</template>

<script>
	export default {
		data() {
			return {
			}
		},
		methods: {
			change(e)
			{
				console.log("值被改变了，值：",e.target.value);
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
