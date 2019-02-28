<script>
export default {
	onLaunch: function() {
		console.log('App Launch');
	},
	onShow: function() {
		console.log('App Show');
	},
	onHide: function() {
		console.log('App Hide');
	}
};
</script>

<style>
/*每个页面公共css */
.bodyFont {
	/* 苹方-简 细体 */
	font-family: PingFangSC-Light, sans-serif;
}
.placeholder {
	font-family: PingFangSC-Ultralight, sans-serif;
	font-size: $uni-font-size-sm;
}
.textTitle {
	/* 苹方-简 常规体 */
	font-family: PingFangSC-Regular, sans-serif;
}
</style>
