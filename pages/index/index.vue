<template>
	<view class="container">
		<view class="intro">本项目已包含uni ui组件，无需import和注册，可直接使用。在代码区键入字母u，即可通过代码助手列出所有可用组件。光标置于组件名称处按F1，即可查看组件文档。</view>
		<text class="intro">详见：</text>
		<button type="default">这是button</button>
		<uni-link :href="href" :text="href"></uni-link>
		<view class="operation">
					<navigator class="list"  url="../../pages/location/location">
						<view class="title">售后服务</view>
					</navigator>
					<navigator class="list"  >
						<view  class="title">积分兑换</view>
					</navigator>
					<navigator class="list"  >
						<view  class="title">会员信息</view>
					</navigator>
					<navigator class="list">
						<view  class="title">关联设备</view>
					</navigator>
					
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				href: 'https://uniapp.dcloud.io/component/README?id=uniui'
			}
		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.container {
		padding: 20px;
		font-size: 14px;
		line-height: 24px;
	}
	.operation{
				margin-top: 54rpx;
				.list{
					box-sizing: border-box;
					padding: 40rpx;
					font-size:32rpx;
					color: #fff;
					width:323rpx;
					height:291rpx;
					float: left;
					margin-bottom: 40rpx;
					background-size: 100% 100%;
					position: relative;
					&:nth-child(odd){
						margin-right:8rpx;
					}
					&:nth-child(1){
						background-image: url(../../static/index/afterAale.png);
					}
					&:nth-child(2){
						background-image: url(../../static/index/exchange.png);
						.title{
							text-align: right;
						}
					}
					&:nth-child(3){
						background-image: url(../../static/index/member.png);
						.title{
							position: absolute;
							left: 40rpx;
							bottom: 40rpx;
						}
					}
					&:nth-child(4){
						background-image: url(../../static/index/binding.png);
						.title{
							position: absolute;
							right: 40rpx;
							bottom: 40rpx;
						}
					}
				}
			}
</style>
