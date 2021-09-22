<template>
	<view class="content">
		<form @submit="formSubmit">
			<view class="uni-form-item">
				<view class="title"><h2>我要上报</h2></view>
				<br/>
				<form @submit="formSubmit">
					<view class="title">1.姓名</view>
					<input id="name" value="王学彬" disabled="true" />
					<br/>
					<view class="title">2.地址</view>
					<input id="addr" value="寿县瓦埠镇西街666号" disabled="true" />
					<br/>
					<view class="uni-form-item uni-column">
						<view class="title">3.是否损坏</view>
						<radio-group name="isBad">
							<label>
								<radio value="1" /><text>是</text>
							</label>
							<label>
								<radio value="0" checked="ture"/><text>否</text>
							</label>
						</radio-group>
					</view>
					<br/>
					<view class="uni-form-item uni-column">
						<view class="title">4.是否堵水</view>
						<radio-group name="isBlocked">
							<label>
								<radio value="1" /><text>是</text>
							</label>
							<label>
								<radio value="0" checked="ture"/><text>否</text>
							</label>
						</radio-group>
					</view>
					<br/>
					<view class="uni-form-item uni-column">
						<view class="title">5.是否清掏</view>
						<radio-group name="isClean">
							<label>
								<radio value="1" /><text>是</text>
							</label>
							<label>
								<radio value="0" checked="ture"/><text>否</text>
							</label>
						</radio-group>
					</view>
					<!-- 拍照上传 -->
					<view class="upload-img">
						<view class="title">拍照上传</view>
						<image src="../../static/images/tabbar/mine.png" 
						style="width: 90rpx; height: 90rpx;"
						@tap="onGetImageClick"></image>
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
				title: '我要上报',
				imageList:[]
			}
		},
		onLoad() {
		},
		methods: {
			formSubmit: function(e) {
				console.log('form发生了submit事件，携带数据为：' + JSON.stringify(e.detail.value))
				var formdata = e.detail.value
				uni.showModal({
					content: '表单数据内容：' + JSON.stringify(formdata),
					showCancel: false
				});
			},
			onGetImageClick(){
				const that = this
				uni.chooseImage({
					count: 6,
					sizeType: ['original', 'compressed'],
					sourceType: ['album', 'camera'],
					success:function(res){
						const len = that.imageList.length
						if(len >= 6) {
							uni.showToast({
								title: '图片最多上传6张'
							})
						}else {
							for(let i = 0; i < 6 -len; i++){
								if(res.tempFilePaths[i]){
									that.imageList.push(res.tempFilePaths[i])
								}
							}
						}
					}
				})
			}
		}
	}
</script>

<style>
	.uni-form-item .title {
		padding: 20rpx 0;
	}
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
