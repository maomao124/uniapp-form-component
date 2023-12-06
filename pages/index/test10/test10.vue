<template>
	<view>
		<picker mode="time" @change="change" start="12:33" end="18:44" @cancel="cancel()">点击时间选择器</picker>
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
