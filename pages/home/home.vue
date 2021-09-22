<template>
	<view class="content">
		<uni-table border stripe emptyText="暂无更多数据" >
		    <!-- 表头行 -->
		    <uni-tr>
		        <uni-th align="center">马桶类型</uni-th>
		        <uni-td>蹲式</uni-td>
		        <uni-th align="center">马桶型号</uni-th>
				<uni-td>MT1001</uni-td>
		    </uni-tr>
		    <uni-tr>
		        <uni-th align="center">安装时间</uni-th>
		        <uni-td>2021年09月17日</uni-td>
				<uni-th align="center">安装地址</uni-th>
				<uni-td>安徽省寿县瓦埠镇街道西街666号</uni-td>
		    </uni-tr>
		    <uni-tr>
		        <uni-th align="center">损坏状态</uni-th>
				<uni-td>正常</uni-td>
				<uni-th align="center">堵水状态</uni-th>
				<uni-td>正常</uni-td>
			</uni-tr>
		    <uni-tr>
		        <uni-th align="center">日常清掏</uni-th>
		        <uni-td>50%</uni-td>
		        <uni-th align="center">维修状态</uni-th>
		        <uni-td>未维修</uni-td>
		    </uni-tr>
		</uni-table>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '我家WC'
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