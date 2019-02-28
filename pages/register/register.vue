<template>
	<view class="bodyFont">
		<view class="uni-padding-wrap uni-common-mt">
			<view class="uni-title uni-common-mt vTitle">注册</view>
			<view class="uni-column-mt viewform"><view class="uni-form-item uni-column vInput">
				<input type="text" value="" class="useInput" placeholder="请输入手机号"
						placeholder-class="placeholder"/>
			</view>
			</view>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {};
	}
};
</script>

<style lang="scss">
$bottomColor: rgb(242, 227, 153);

.viewform {
	padding: 20upx;
}
.vTitle {
	text-align: center;
}
.vInput {
	border-bottom-style: solid;
	border-bottom-width: 0.01em;
	border-color: $bottomColor;
}
.useInput {
	padding: 50upx 50upx 0upx 50upx;
	font-size: $uni-font-size-sm;
}
</style>
