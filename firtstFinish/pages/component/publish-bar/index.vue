<template>
	<view>
		<view class="container" :style="{'background-color': bgColor}">
			<view class="left">+</view>
			<view class="right">
				<view class="top">
					<slot name="title"></slot></view>
				<view class="down">
					<view><slot name="label1"></slot></view>
					<view><slot name="label2"></slot></view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		props:{
			bgColor:{
				type:String,
				default:function(){
					return "#55aaff"
				}
			}
		},
		methods: {

		}
	}
</script>

<style>
	.container{
		border-radius: 10upx;
		display: flex;
		padding: 20upx;
	}
	.left {				
		display: flex;
		align-self: center;
		color:#FFFFFF;
		font-size: 40upx;
		margin-right:20upx ;
		font-weight: bold;
	}
	.right .top{
		color:#FFFFFF;
		font-size: 40upx;
		font-weight: bold;
	}
	.right .down{
		display: flex;
		flex-direction: column;
		color: #B9DFF9;
		font-size:25upx;
	}
</style>
