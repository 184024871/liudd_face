<template>
	<view class="content">
		<!-- 标题 -->
		<view>
			<text>上报记录</text>
		</view>
		<!-- 上报记录列表 -->
		<view style="width: 100%;">
			<uni-table  border stripe emptyText="暂无更多数据" >
				<uni-tr>
					<uni-th align="center">序号</uni-th>
					<uni-th align="center">损坏类型</uni-th>
					<uni-th align="center">上报时间</uni-th>
					<uni-th align="center">维修状态</uni-th>
				</uni-tr>
				<uni-tr>
					<uni-td align="center">1</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已上报</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">2</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已维修</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">3</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">4</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">5</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">6</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">7</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">8</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">9</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr><uni-tr>
					<uni-td align="center">10</uni-td>
					<uni-td align="center">堵水</uni-td>
					<uni-td align="center">2021年9月22日</uni-td>
					<uni-td align="center">已评价</uni-td>
				</uni-tr>
			</uni-table>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '上报记录'
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
