<template>
	<view>
		<!-- 轮播图组件 -->
		<swiper-image :resdata="swipers"></swiper-image>
		<!-- 首页分类 -->
		<indexNav :resdata="indexnavs"></indexNav>
		<!-- 全局分割线 -->
		<divider></divider>
		<!-- 三图广告 -->
		<threeAdv :resdata="threeAdv"></threeAdv>
		
		<divider></divider>
		<!-- 基础卡片组件 -->
		<card  headTitle="每日精选" bodyCover="/static/images/demo/demo4.jpg"></card>
		
		<!-- 公共列表组件 750-5=745/2=372.5 -->
		<view class="row">
			<view style="width:372.5rpx;" class="">
				<image src="../../static/images/demo/list/1.jpg" mode="widthFix" lazy-load></image>
				<view class="p-2 pt-1">
					<view class="font-md">米家空调</view>
					<text class="d-block font text-light-muted">1.5匹变频</text>
					<view class="d-flex my-1">
						<view class="d-flex main-text-color font-md line-h">
							<text class="a-self-start font-sm" style="">￥</text>1366
						</view>
						<view class="font-sm text-light-muted line-through ml-1 line-h" style="align-content: flex-end ;">￥2699</view>
					</view>
				</view>
				
			</view>
		</view>
		<view style="height:100rpx;"></view>
	</view>  
	
</template>

<script>
	import swiperImage from "@/components/index/swiper-image.vue"
	import indexNav from "@/components/index/index-nav.vue"
	import threeAdv from "@/components/index/three-adv.vue"
	import card from "@/components/common/card.vue"
	
	
	export default {
		components:{
			swiperImage,
			indexNav,
			threeAdv,
			card
		},
		data() {
			return {
				swipers:[
					{src:"../../static/images/demo/demo4.jpg",},
					{src:"../../static/images/demo/demo5.jpg",},
					{src:"../../static/images/demo/demo6.jpg",}
				],
				indexnavs:[
					{src:"/static/images/indexnav/1.png",text:"新品发布"},
					{src:"/static/images/indexnav/2.gif",text:"小米众筹"},
					{src:"/static/images/indexnav/3.gif",text:"以旧换新"},
					{src:"/static/images/indexnav/4.gif",text:"一分拼团"},
					{src:"/static/images/indexnav/5.gif",text:"超值特卖"},
					{src:"/static/images/indexnav/6.gif",text:"一分秒杀"},
					{src:"/static/images/indexnav/7.gif",text:"真心想要"},
					{src:"/static/images/indexnav/8.gif",text:"电视热卖"},
					{src:"/static/images/indexnav/9.gif",text:"家电热卖"},
					{src:"/static/images/indexnav/10.gif",text:"米粉卡"},
				],
				threeAdv:{
					big:{
						src:"/static/images/demo/demo2.jpg"
					},
					samlltop:{
						src:"/static/images/demo/demo2.jpg"
					},
					smallbottom:{
						src:"/static/images/demo/demo2.jpg"
					}
				}
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
