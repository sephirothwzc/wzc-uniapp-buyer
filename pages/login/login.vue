<template>
	<view class="bodyFont">
		<!-- #ifdef APP-PLUS 占位符 navbar -->
		<view class="status_bar"><view class="top_view"></view></view>
		<!-- #endif -->
		<view class="uni-padding-wrap uni-common-mt">
			<view class="uni-title uni-common-mt viewTitle textTitle">登陆</view>
			<view class="uni-column-mt viewform">
				<view class="uni-form-item uni-column viewinput">
					<input
						type="text"
						value=""
						class="uni-input useinput"
						placeholder="请输入账户名"
						placeholder-class="placeholder"
					/>
				</view>
				<view
					class="uni-form-item uni-column;"
					style="border-bottom: solid 0.01em;border-color:rgb(242, 227, 153);"
				>
					<text style="float:right;" class="useForgetPW">忘记密码</text>
					<input
						type="text"
						value=""
						class="uni-input useinput"
						placeholder="请输入密码"
						placeholder-class="placeholder"
					/>
				</view>
				<view class="uni-form-item uni-column viewButton">
					<button type="primary" class="useButton">
						<text style="color: black;">登&nbsp;&nbsp;陆</text>
					</button>
				</view>
				<view class="uni-form-item uni-column viewText">
					<text style="float: right;">短信验证码登陆</text>
					<navigator url="/pages/register/register"><text>注册</text></navigator>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
/**
 * 登陆
 */
export default {
	data() {
		return {};
	}
};
</script>

<style lang="scss">
$bottomColor: rgb(242, 227, 153);
.viewTitle {
	padding-top: 50upx;
	padding-left: 15upx;
	font-size: $uni-font-size-lg;
}
.viewform {
	padding: 20upx;
}
.viewinput {
	border-bottom-style: solid;
	border-bottom-width: 0.01em;
	border-color: $bottomColor;
}
.viewText {
	padding-top: 20upx;
	font-size: $uni-font-size-sm;
}
.useinput {
	padding: 50upx 50upx 0upx 50upx;
	font-size: $uni-font-size-sm;
}
.useForgetPW {
	font-size: $uni-font-size-sm;
	padding: 60upx 0upx 0upx 0upx;
}
.viewButton {
	padding-top: 80upx;
}
.useButton {
	height: 100upx;
	vertical-align: middle;
	padding-top: 20upx;
	font-size: $uni-font-size-base;
	background-color: $bottomColor;
	color: rgb(255, 255, 255);
}
/**
 * app-plus
 */
.status_bar {
	height: var(--status-bar-height);
	width: 100%;
	background-color: #f8f8f8;
}
.top_view {
	height: var(--status-bar-height);
	width: 100%;
	position: fixed;
	background-color: #f8f8f8;
	top: 0;
	z-index: 999;
}
</style>
