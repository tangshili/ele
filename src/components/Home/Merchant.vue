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
					<span class="merchant-inflrmatin-open" v-text="item.open"></span>
				</div>
				<i style="color:#FFD800; margin-top:10px;" class="fa" :class="item.icon1"></i>
				<i style="color:#FFD000;" class="fa" :class="item.icon2"></i>
				<i style="color:#FFC700;" class="fa" :class="item.icon3"></i>
				<i style="color:#FFBD00;" class="fa" :class="item.icon4"></i>
				<i style="margin-right:8px; color:#FFB200;" class="fa" :class="item.icon5"></i>
				<span style="font-size:12px; color:#333333;" v-text="item.score"></span>
				<span style="margin-left:3px; font-size:12px; color:#333333; display:inline-block;" v-text="item.number"></span>
				<div class="Delivery" v-text="item.delivery"></div>
				<div v-text="item.null"></div>
				<div style="font-size:12px; color:#333333; margin-top:12px; display:inline-block;" v-text="item.start"></div>
				<span style="color:#999; margin:0px 3px;" v-text="item.line"></span>
				<span style="font-size:12px; color:#333333;" v-text="item.start"></span>
				<div style="font-size:12px; color:#666666; float:right; margin-top:10px;" v-text="item.distance"></div>
				<span style="color:#ccc; margin:6px 3px; float:right;" v-text="item.line"></span>
				<span style="font-size:12px; color:#666666; float:right; margin-top:10px;" v-text="item.time"></span>
				<div class="Varieties" v-text="item.Varieties"></div>
				<div class="full" v-text="item.full"></div>
				<span style="margin-top: 12px;font-size: 12px;" v-text="item.Full"></span>
				<i style="font-size:14px; margin-left:5px; float:right;" class="fa" :class="item.caretDown"></i>
				<span class="activity" v-text="item.activity"></span><br />
				<div class="special" v-text="item.special"></div>
				<span style="font-size:12px;" v-text="item.Special"></span><br />
				<div class="first" v-text="item.first"></div>
				<span style="font-size:12px;" v-text="item.First"> </span>
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
					time: '20分钟',
					Varieties: '奶茶果汁',
					full: '满',
					Full: '满25减4',
					caretDown: 'fa-care-down',
					activity: '3个活动',
					special: '特',
					Special: '9.9秒杀！焦糖茶拿铁(限12:00-17:00)',
					first: '首',
					First: '新用户下单立减17元',
					null:''
				},{
					title: '品牌',
					image: require('../../assets/images/food-1.png'),
					name: '元祖蛋糕（宝山店）',
					logo: 'Ganso',
					open: '...',
					icon1: 'fa-star',
					icon2: 'fa-star',
					icon3: 'fa-star',
					icon4: 'fa-star',
					icon5: 'fa-star',
					score: '4.9',
					number: '月售198单',
//					delivery: '蜂鸟专送',
					start: '￥100元起送',
					freight: '免配送费',
					line: '|',
					distance: '2.41公里',
					time: '41分钟',
					Varieties: '甜品',
					full: '满',
					Full: '满5减5',
					caretDown: 'fa-care-down',
					activity: '3个活动',
					special: '特',
					Special: '单品定价',
					first: '首',
					First: '新用户下单立减17元',
					null:''
				},{
					title: '品牌',
					image: require('../../assets/images/food-2.png'),
					name: '鹿角巷(牡丹旗舰店)',
					logo: '鹿角巷',
					open: '...',
					icon1: 'fa-star',
					icon2: 'fa-star',
					icon3: 'fa-star',
					icon4: 'fa-star',
					icon5: 'fa-star',
					score: '4.9',
					number: '月售2126单',
//					delivery: '蜂鸟专送',
					start: '￥0元起送',
					freight: '远距离配送费￥4',
					line: '|',
					distance: '3.26公里',
					time: '42分钟',
					Varieties: '奶茶果汁',
					full: '满',
					Full: '满35减5，满60减10，满100减20，满…',
					caretDown: 'fa-care-down',
					activity: '17个活动',
					special: '折',
					Special: '单品定价',
					first: '新',
					First: '本店新用户下单立减1元',
					null:''
				},{
					title: '品牌',
					image: require('../../assets/images/food-2.png'),
					name: '鹿角巷(牡丹旗舰店)',
					logo: '鹿角巷',
					open: '...',
					icon1: 'fa-star',
					icon2: 'fa-star',
					icon3: 'fa-star',
					icon4: 'fa-star',
					icon5: 'fa-star',
					score: '4.9',
					number: '月售2126单',
//					delivery: '蜂鸟专送',
					start: '￥0元起送',
					freight: '远距离配送费￥4',
					line: '|',
					distance: '3.26公里',
					time: '42分钟',
					Varieties: '奶茶果汁',
					full: '满',
					Full: '满35减5，满60减10，满100减20，满…',
					caretDown: 'fa-care-down',
					activity: '17个活动',
					special: '折',
					Special: '单品定价',
					first: '新',
					First: '本店新用户下单立减1元',
					null:''
				},{
					title: '品牌',
					image: require('../../assets/images/food-2.png'),
					name: '鹿角巷(牡丹旗舰店)',
					logo: '鹿角巷',
					open: '...',
					icon1: 'fa-star',
					icon2: 'fa-star',
					icon3: 'fa-star',
					icon4: 'fa-star',
					icon5: 'fa-star',
					score: '4.9',
					number: '月售2126单',
//					delivery: '蜂鸟专送',
					start: '￥0元起送',
					freight: '远距离配送费￥4',
					line: '|',
					distance: '3.26公里',
					time: '42分钟',
					Varieties: '奶茶果汁',
					full: '满',
					Full: '满35减5，满60减10，满100减20，满…',
					caretDown: 'fa-care-down',
					activity: '17个活动',
					special: '折',
					Special: '单品定价',
					first: '新',
					First: '本店新用户下单立减1元',
					null:''
				}]
			}
		}
	}
</script>

<style>
	.merchant {
		width: 100%;
		height: 230px;
		padding: 15px 10px 10px;
		box-sizing: border-box;
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
	
	.fa {
		font-size: 12px;
	}
	
	.Delivery {
		font-size: 12px;
		float: right;
		color: white;
		background-color: #009BFF;
		border-radius: 2px;
		padding: 2px;
	}
	
	.Varieties {
		font-size: 12px;
		border: 1px solid #EEEEEE;
		border-radius: 2px;
		padding: 3px;
		width: 58px;
		margin: 12px 0px 24px;
		box-sizing: border-box;
	}
	
	.full {
		background-color: #F07373;
		border-radius: 2px;
		padding: 1px 2px;
		color: #FFFFFF;
		font-size: 12px;
		margin-right: 5px;
		margin-top: 6px;
		display: inline-block;
		margin-bottom: 6px;
	}
	
	.special {
		background-color: #F1884F;
		border-radius: 2px;
		padding: 1px 2px;
		color: #FFFFFF;
		font-size: 12px;
		margin-right: 5px;
		margin-bottom: 6px;
		display: inline-block;
	}
	
	.first {
		background-color: #70BC46;
		border-radius: 2px;
		padding: 1px 2px;
		color: #FFFFFF;
		font-size: 12px;
		margin-right: 5px;
		margin-bottom: 6px;
		display: inline-block;
	}
	
	.activity {
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