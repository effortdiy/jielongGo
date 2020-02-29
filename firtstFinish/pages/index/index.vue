<template>
	<view>
		<view class="row2">
			<view>
				<publishBar bgColor="#62BDFA">
					<block slot="title">反馈接龙</block>
					<block slot="label1">通知 公告 反馈 确认</block>
					<block slot="label2">作业 抢单 打卡 留档</block>
				</publishBar>
			</view>
			<view>
				<publishBar bgColor="#5288F8">
					<block slot="title">填表接龙</block>
					<block slot="label1">信息手机 数据统计 工作</block>
					<block slot="label2">汇报 阅读打卡 拼单代购</block>
				</publishBar>
			</view>
		</view>
		<view class="row1">
			<publishBar bgColor="#F45537">
				<block slot="title">团购接龙</block>
				<block slot="label1">轻松管理订单和收款,自由选择自提或物流</block>
			</publishBar>
		</view>
		<view class="row2">
			<view>
				<publishBar bgColor="#9D46FD">					
					<block slot="title">活动接龙</block>
					<block slot="label1">报名 培训 团建 聚会</block>
					<block slot="label2">招募 订餐 试吃 旅游</block>
				</publishBar>
			</view>
			<view>
				<publishBar bgColor="#FFBC32">
					<block slot="title">调查评选</block>
					<block slot="label1">调查 评选 决议</block>
					<block slot="label2">征集</block>
				</publishBar>
			</view>
		</view>
	</view>
</template>

<script>
	import publishBar from '@/pages/component/publish-bar/index'
	export default {
		components: {
			publishBar
		},
		data() {
			return {

			}
		},
		props: {},
		methods: {

		}
	}
</script>

<style>	
	.row2 {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		padding: 10upx 20upx;
	}
	.row2 view{
		width: 45vw;
	}
	.row1 {		
		padding: 10upx 20upx;
	}
	.row1 view{
		
	}
</style>
