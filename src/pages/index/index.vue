<template>
	<view class="content">
		<view class="topbar">
			<view class="avatar">
				<open-data type="userAvatarUrl"></open-data>
			</view>
			<view class="info">
				<text>你好，</text>
				<open-data type="userNickName"></open-data>
			</view>
		</view>
		<image class="logo" src="/static/logo.png"></image>
		<view class="title">
			<text>{{title}}</text>
		</view>
		<view class="subtitle">
			<text>{{subtitle}}</text>
		</view>
		<view class="nav">
			<navigator url="/pages/miniapp/index" class="nav-btn" hover-class="navigator-hover">
				<button type="primary">小程序开发</button>
			</navigator>
			<navigator url="/pages/contact/index" class="nav-btn" hover-class="navigator-hover">
				<button type="default">联系方式</button>
			</navigator>
			<navigator url="/pages/about/index" class="nav-btn" hover-class="navigator-hover">
				<button type="default">关于我</button>
			</navigator>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '皆鸣开发',
				subtitle: '鏦鏦铮铮  金铁皆鸣'
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

	.logo {
		height: 240rpx;
		width: 240rpx;
		margin: 100rpx auto 60rpx auto;
	}

	.topbar {
		display: flex;
		flex-direction: row-reverse;
		width: 100%;
	}

	.info {
		margin: 3px 0;
		font-size: 12px;
		color: #888;
	}

	.avatar {
		overflow:hidden;  
		width: 40rpx;
		height: 40rpx;
		margin: 5rpx;
		border-radius: 100%;
		box-shadow: 1px 1px 5px rgba(0, 0, 0, 0.2);
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 24px;
		margin-bottom: 30px;
		color: #aa1313;
		font-weight: 300;
		letter-spacing: 3px;
	}
	.subtitle {
		margin-bottom: 10px;
		font-size: 12px;
		font-weight: 300;
		letter-spacing: 8px;
		color: #b17878
	}
	.nav {
		width: 100%;
	}
	.nav-btn {
		margin: 10px;
	}
</style>
