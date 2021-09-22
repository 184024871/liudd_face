<template>
	<view class="content">
		<!-- 我的头像 -->
		<view>
			<text style="margin: 30rpx;">王学彬</text><image src="../../static/logo.png" style="width: 90rpx; height: 90rpx; float: left;margin: 30rpx;"></image>
			<br>
			<text>寿县瓦埠镇街道西街666号</text>
		</view>
		<!-- 我的地址 -->
		<view>
		</view>
		<!-- 我的手机号 -->
		<view>
			<text>我的手机：19956566666</text>
		</view>
		<!-- 密码修改 -->
		<view>
			<text>修改密码</text>
		</view>
		<!-- 退出登录 -->
		<view>
			<text>退出登录</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '我的'
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
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}
	
	.text-area {
		display: flex;
		justify-content: center;
	}
	
	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
