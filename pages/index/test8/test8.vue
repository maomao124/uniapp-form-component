<template>
	<view>
		<picker mode="multiSelector" :range="data" @change="change" @cancel="cancel()">点击多列选择器</picker>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				data: [
					['1', '2', '3', '4', '5'],
					['6', '7', '8', '9', '10'],
					['11', '12', '13', '14', '15']
				],
			}
		},
		methods: {
			change(e) {
				console.log("值被改变了，索引：", e.target.value, "值：",
					this.data[0][e.target.value[0]],
					this.data[1][e.target.value[1]],
					this.data[2][e.target.value[2]]);
			},
			cancel() {
				console.log("取消");
			}
		}
	}
</script>

<style>

</style>