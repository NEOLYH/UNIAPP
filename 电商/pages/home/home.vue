<template>
	<view class="box">
		<view>1234564564</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				city: ''
			}
		},
		onLoad: function() {
			// #ifdef APP-PLUS
			this.nVueTitle = uni.getSubNVueById('homeTitleNvue');
			this.nVueTitle.onMessage(res => {
				let type = res.data.type;
				if (type == 'focus') {

				}
			});
			this.nVueTitle.postMessage({
				city: '噢哟'
			});
			// #endif	
		},
		methods: {

		}
	}
</script>

<style>
	page {
		width: 100%;
		height: 100%;
	}

	.box {
		width: 100%;
		height: 100%;
		background-color: #4CD964;
	}
</style>
