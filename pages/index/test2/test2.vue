<template>
	<view>
		<checkbox-group @change="c">
			<checkbox value="1">内容1</checkbox>
			<checkbox value="2">内容2</checkbox>
			<checkbox value="3">内容3</checkbox>
			<checkbox value="4">内容4</checkbox>
		</checkbox-group>
		<checkbox-group>
			<checkbox value="1">内容1</checkbox>
			<checkbox value="2" checked="true">内容2</checkbox>
			<checkbox value="3" checked="true">内容3</checkbox>
		</checkbox-group>
		<checkbox-group>
			<checkbox value="1">内容1</checkbox>
			<checkbox value="2" checked="true" disabled="true">内容2</checkbox>
			<checkbox value="3" disabled="true">内容3</checkbox>
		</checkbox-group>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			c(e)
			{
				console.log(e);
				console.log(e.target.value);
			}
		}
	}
</script>

<style>

</style>
