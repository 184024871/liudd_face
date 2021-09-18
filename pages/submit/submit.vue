<template>
	<view class="content">
		<form @submit="formSubmit" @reset="formReset">
			<view class="uni-form-item">
				
				<view class="title"><h2>我要上报</h2></view>
				<br/>
				<form @submit="formSubmit" @reset="formReset">
					<view class="title">1.姓名</view>
					<input value="王学彬" disabled="true" />
					<br/>
					<view class="title">2.地址</view>
					<input value="寿县瓦埠镇西街666号" disabled="true" />
					<br/>
					<view class="uni-form-item uni-column">
						<view class="title">3.是否损坏</view>
						<radio-group name="radio">
							<label>
								<radio value="radio1" /><text>是</text>
							</label>
							<label>
								<radio value="radio2" checked="ture"/><text>否</text>
							</label>
						</radio-group>
					</view>
					<br/>
					<view class="uni-form-item uni-column">
						<view class="title">4.是否堵水</view>
						<radio-group name="radio">
							<label>
								<radio value="radio1" /><text>是</text>
							</label>
							<label>
								<radio value="radio2" checked="ture"/><text>否</text>
							</label>
						</radio-group>
					</view>
					<br/>
					<view class="uni-form-item uni-column">
						<view class="title">5.是否清掏</view>
						<radio-group name="radio">
							<label>
								<radio value="radio1" /><text>是</text>
							</label>
							<label>
								<radio value="radio2" checked="ture"/><text>否</text>
							</label>
						</radio-group>
					</view>
					<br/>
					<view class="uni-btn-v">
						<button form-type="submit">提交</button>
					</view>
				</form>
			</view>
		</form>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '我要上报'
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
