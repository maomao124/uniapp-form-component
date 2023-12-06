<template>
	<view>
		<view>
			<slider value="60" @change="sliderChange" />
		</view>
		<view>
			<slider value="60" @change="sliderChange" show-value />
		</view>
		<view>
			<slider value="240" min="100" max="3000" @change="sliderChange" show-value />
		</view>
		<view>
			<slider value="60" step="10" @change="sliderChange" show-value/>
		</view>
		<view>
			<slider value="44" disabled="true" @change="sliderChange" show-value />
		</view>
		<view>
			<slider value="60" @change="sliderChange" active-color="red" background-color="green" show-value />
		</view>
		<view>
			<slider value="72" @change="sliderChange" 
			active-color="red" background-color="green"
			block-color="skyblue" show-value />
		</view>
		<view>
			<slider value="45" @change="sliderChange" 
			active-color="red" background-color="green"
			block-color="skyblue" block-size="12" show-value />
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
			sliderChange(e)
			{
				console.log(e.detail.value);
			}
		}
	}
</script>

<style>

</style>
