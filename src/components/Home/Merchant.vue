<template>
	<div class="merchant-box">
		<div class="merchant weui-flex" v-for="(item,index) in merchant">
			<div class="merchant-log">
				<img :src="item.image" />
			</div>
			<div class="merchant-information" style="flex:1">
				<div class="merchant-informatin-title">
					<span class="merchant-informatin-brand" v-text="item.title"></span>
					<span class="merchant-inflrmatin-logo" v-text="item.name"><span style="font-weight: bold;" v-text="item.logo"></span></span>
					<span class="merchant-inflrmatin-open"></span>
				</div>
				<div class="merchant-sales-volume">
					<i style="color:#FFD800;" class="fa" :class="item.icon1"></i>
					<i style="color:#FFD000;" class="fa" :class="item.icon2"></i>
					<i style="color:#FFC700;" class="fa" :class="item.icon3"></i>
					<i style="color:#FFBD00;" class="fa" :class="item.icon4"></i>
					<i style="margin-right:8px; color:#FFB200;" class="fa" :class="item.icon5"></i>
					<span style="font-size:12px; color:#333333;" v-text="item.score"><span style="margin-left:3px;" v-text="item.number"></span> </span>
					<span class="Delivery" v-text="item.delivery"></span>
				</div>
				<div class="Distribution-fee">
					<span style="font-size:12px; color:#333333;" v-text="item.start"><span style="color:#999; margin:0px 3px;" v-text="item.line"></span><span style="font-size:12px; color:#333333;" v-text="item.freight"></span> </span>
					<span style="font-size:12px; color:#666666; float:right;" v-text="item.distance"><span style="color:#ccc; margin:0px 3px;" v-text="item.line"></span><span style="font-size:12px; color:#666666;" v-text="item.time"></span></span>
				</div>
				<div class="Varieties">奶茶果汁</div>
				<div class="Full-reduction">
					<span class="full">满</span>满25减4
					<div class="activity">3个活动<i style="font-size:14px; margin-left:5px;" class="fa fa-caret-down"></i></div>
				</div>
				<div class="Full-reduction">
					<span class="special">特</span>9.9秒杀！焦糖茶拿铁(限12:00-17:00)
				</div>
				<div class="Full-reduction">
					<span class="first">首</span>新用户下单立减17元
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				merchant: [{
					title: '品牌',
					image: require('../../assets/images/coco-logo.png'),
					name: '都可(清溪)',
					logo: 'CoCo',
					open: '...',
					icon1: 'fa-star',
					icon2: 'fa-star',
					icon3: 'fa-star',
					icon4: 'fa-star',
					icon5: 'fa-star',
					score: '4.9',
					number: '月售946单',
					delivery: '蜂鸟专送',
					start: '￥20元起送',
					freight: '配送费￥5.3',
					line: '|',
					distance: '903米',
					time:'20分钟'
				}]
			}
		}
	}
</script>

<style>
	.merchant {
		width: 100%;
		height: 200px;
		padding: 15px 10px 10px;
		box-sizing: border-box;
		margin-bottom: 100px;
		box-sizing: border-box;
		border-bottom: 1px solid #EEEEEE;
	}
	
	.merchant-log {
		width: 80px;
	}
	
	.merchant-log img {
		width: 80px;
	}
	
	.merchant-information {
		width: 100%;
		padding-left: 10px;
		box-sizing: border-box;
	}
	
	.merchant-informatin-brand {
		font-size: 12px;
		padding: 3px;
		background-color: #FFEC13;
		border-radius: 3px;
		color: #855A15;
		display: inline-block;
		width: 24px;
	}
	
	.merchant-inflrmatin-logo {
		margin-left: 5px;
		font-size: 16px;
	}
	
	.merchant-inflrmatin-open {
		float: right;
		font-size: 20px;
		line-height: 3px;
	}
	
	.merchant-sales-volume {
		margin-top: 5px;
	}
	
	.merchant-sales-volume .fa {
		font-size: 12px;
	}
	
	.merchant-sales-volume .Delivery {
		font-size: 12px;
		float: right;
		color: white;
		background-color: #009BFF;
		border-radius: 2px;
		padding: 2px;
	}
	
	.Distribution-fee {
		margin-top: 5px;
	}
	
	.Varieties {
		font-size: 12px;
		border: 1px solid #EEEEEE;
		border-radius: 2px;
		padding: 3px;
		width: 58px;
		margin-top: 8px;
		box-sizing: border-box;
	}
	
	.Full-reduction {
		margin-top: 12px;
		font-size: 12px;
	}
	
	.Full-reduction .full {
		background-color: #F07373;
		border-radius: 2px;
		padding: 1px 2px;
		color: #FFFFFF;
		font-size: 12px;
		margin-right: 5px;
	}
	
	.Full-reduction .special {
		background-color: #F1884F;
		border-radius: 2px;
		padding: 1px 2px;
		color: #FFFFFF;
		font-size: 12px;
		margin-right: 5px;
	}
	
	.Full-reduction .first {
		background-color: #70BC46;
		border-radius: 2px;
		padding: 1px 2px;
		color: #FFFFFF;
		font-size: 12px;
		margin-right: 5px;
	}
	
	.Full-reduction .activity {
		font-size: 12px;
		float: right;
	}
</style>

<!--<div class="merchant weui-flex">
	<div class="merchant-log">
		<img src="../../assets/images/coco-logo.png" />
	</div>
	<div class="merchant-information" style="flex:1">
		<div class="merchant-informatin-title">
			<span class="merchant-informatin-brand">品牌</span>
			<span class="merchant-inflrmatin-logo"><span style="font-weight: bold;">CoCo</span> 都可(清溪)</span>
			<span class="merchant-inflrmatin-open">...</span>
		</div>
		<div class="merchant-sales-volume">
			<i style="color:#FFD800;" class="fa fa-star"></i>
			<i style="color:#FFD000;" class="fa fa-star"></i>
			<i style="color:#FFC700;" class="fa fa-star"></i>
			<i style="color:#FFBD00;" class="fa fa-star"></i>
			<i style="margin-right:8px; color:#FFB200;" class="fa fa-star"></i>
			<span style="font-size:12px; color:#333333;">4.9&nbsp;&nbsp;月售946单</span>
			<span class="Delivery">蜂鸟专送</span>
		</div>
		<div class="Distribution-fee">
			<span style="font-size:12px; color:#333333;">￥20元起送<span style="color:#999; margin:0px 3px;">|</span>配送费￥5.3</span>
			<span style="font-size:12px; color:#666666; float:right;">903米<span style="color:#ccc; margin:0px 3px;">|</span>20分钟</span>
		</div>
		<div class="Varieties">奶茶果汁</div>
		<div class="Full-reduction">
			<span class="full">满</span>满25减4
			<div class="activity">3个活动<i style="font-size:14px; margin-left:5px;" class="fa fa-caret-down"></i></div>
		</div>
		<div class="Full-reduction">
			<span class="special">特</span>9.9秒杀！焦糖茶拿铁(限12:00-17:00)
		</div>
		<div class="Full-reduction">
			<span class="first">首</span>新用户下单立减17元
		</div>
	</div>
</div>-->