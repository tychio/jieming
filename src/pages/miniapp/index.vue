<template>
	<view class="content">
		<view class="description">
			<text>{{description}}</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				description: '可定制开发多平台小程序，使用先进的前端开发框架Vue开发，在各种设备上渲染流畅。利用Uniapp打包工具可一套代码发布各大主流小程序平台。包括微信，支付宝，百度，字节跳动，快应用，QQ，360，快手，飞书等。'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.description {
		padding: 10px;
		text-indent: 30px;
	}
</style>
