<template>
	<view>
		<radio-group @change="change">
			<radio value="1">单选框1</radio>
			<radio value="2">单选框2</radio>
			<radio value="3">单选框3</radio>
		</radio-group>
		<radio-group @change="change">
			<radio value="1">单选框1</radio>
			<radio value="2">单选框2</radio>
			<radio value="3" disabled="true">单选框3</radio>
		</radio-group>
		<radio-group @change="change">
			<radio value="1" checked="true">单选框1</radio>
			<radio value="2">单选框2</radio>
			<radio value="3">单选框3</radio>
		</radio-group>
		<radio-group @change="change">
			<radio value="1" color="#aaff00">单选框1</radio>
			<radio value="2" color="#aaff00">单选框2</radio>
			<radio value="3" color="#aaff00">单选框3</radio>
		</radio-group>
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
				console.log(e);
				console.log("当前选择的是：",e.detail.value);
			}
		}
	}
</script>

<style>

</style>
