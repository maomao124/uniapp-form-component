<template>
	<view>
		<scroll-view scroll-y="true">
			<view>
				<view class="title">input</view>
				<input placeholder="输入框"/>
			</view>
			<view>
				<view class="title">焦点输入框</view>
				<input focus="true" placeholder="焦点输入框"/>
			</view>
			<view>
				<view class="title">最大长度为5的输入框</view>
				<input maxlength="5" placeholder="最大长度为5的输入框"/>
			</view>
			<view>
				<view class="title">数字输入框</view>
				<input type="number" placeholder="数字输入框"/>
			</view>
			<view>
				<view class="title">小数点数字输入框</view>
				<input type="digit" placeholder="小数点数字输入框"/>
			</view>
			<view>
				<view class="title">身份证输入框</view>
				<input type="idcard" placeholder="身份证输入框"/>
			</view>
			<view>
				<view class="title">电话输入框</view>
				<input type="tel" placeholder="电话输入框"/>
			</view>
			<view>
				<view class="title">密码输入框</view>
				<input type="safe-password" placeholder="密码输入框"/>
			</view>
			<view>
				<view class="title">昵称输入框</view>
				<input type="nickname" placeholder="昵称输入框"/>
			</view>
			<view>
				<view class="title">密码输入框</view>
				<input password="true" placeholder="密码输入框"/>
			</view>
			
			<view>
				<view class="title">禁用输入框</view>
				<input disabled="true" placeholder="禁用输入框" value="123"/>
			</view>
			
			
		</scroll-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		methods: {

		}
	}
</script>

<style>

</style>