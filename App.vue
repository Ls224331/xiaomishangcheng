<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	@import "/common/uni.css";
	/* 动画库 */
	@import "/common/animate.css";
	@import "/common/icon.css";
	/* 公共样式 */
	@import "/common/common.css";
	/* ui基础库 */
	@import "/common/zcm-main.css";
</style>
