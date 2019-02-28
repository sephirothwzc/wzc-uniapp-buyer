<template>
	<view class="content">
		<image class="logo" src="../../static/logo.png"></image>
		<view>
			<text class="title">{{ title }}</text>
			<button @tap="toTest">登陆</button>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			title: 'Hello'
		};
	},
	onLoad() {},
	methods: {
		toTest() {
			uni.navigateTo({
				url: '/pages/login/login',
				success: res => {},
				fail: () => {},
				complete: () => {}
			});
		}
	}
};
</script>

<style>
.content {
	text-align: center;
	height: 400upx;
}
.logo {
	height: 200upx;
	width: 200upx;
	margin-top: 200upx;
}
.title {
	font-size: 36upx;
	color: #8f8f94;
}
</style>
