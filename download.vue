<template>
	<view>
		<web-view :webview-styles="webviewStyles" src="https://wangfeng351.github.io/github-pages-demo/"></web-view>
	</view>
</template>

<script>
	export default {
	        data() {
	            return {
	                webviewStyles: {
	                    progress: {
	                        color: '#FF3333'
	                    },
						flex: 1
	                },
					url: '../../hybrid/html/index.html'
	            }
	        },
	        onLoad(options) {
	        },
	        //监听html返回上一页的事件 跳转到相对于的页面
	        onBackPress(options) {
				// if(options.from === 'backbutton') {
				// 	uni.redirectTo({
				// 		url: `/pages/login/login`
				// 	});
				// } 
			},
	    }
</script>

<style>
</style>