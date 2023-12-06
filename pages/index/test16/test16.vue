<template>
	<view>
		<view>
			<textarea @input="change"></textarea>
		</view>
		<view>
			<textarea @input="change" auto-height="true"></textarea>
		</view>
		<view>
			<textarea @input="change" maxlength="9999" auto-height="true"></textarea>
		</view>
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
				console.log("长度：",e.detail.value.length,'值:',e.detail.value);
			}
		}
	}
</script>

<style>
textarea{
	background-color: bisque;
	margin: 2ch;
}
</style>
