<template>
	<!-- 左边 373 530 -->
	<!-- 右边 375 264 边高2-->
	<view class="d-flex">
		<image :src="resdata.big.src" mode="" lazy-load style="width:373rpx;height: 530rpx;border-right: 2rpx solid #F5F5F5;" @tap="event(resdata.big)"></image>
		<view class="d-flex flex-column">
			<image :src="resdata.samlltop.src" style="width:375rpx;height: 264rpx;border-bottom:2rpx solid #F5F5F5" mode="" @tap="event(resdata.samlltop)"></image>
			<image :src="resdata.smallbottom.src" style="width:375rpx;height: 264rpx;" mode="" @tap="event(resdata.smallbottom)"></image>
		</view>
	</view>
</template>

<script>
	export default{
		props:{
			resdata:Object
		},
		methods:{
			event(obj){
				console.log("点击了三图")
			}
		}
	}
</script>

<style>
</style>
