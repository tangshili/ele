<template>
	<div class="merchant weui-flex">
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
		</div>
	</div>
</template>

<script>
</script>

<style>
	.merchant {
		width: 100%;
		height: 280px;
		padding: 10px;
		box-sizing: border-box;
		background-color: #0085FF;
		margin-bottom: 100px;
		box-sizing: border-box;
	}
	
	.merchant-log {
		width: 80px;
		height: 260px;
		background-color: gold;
	}
	
	.merchant-log img {
		width: 80px;
	}
	
	.merchant-information {
		width: 100%;
		height: 260px;
		background-color: deeppink;
		padding-left: 5px;
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
	.merchant-sales-volume{
		margin-top:5px;
	}
	.merchant-sales-volume .fa{
		font-size:12px;
	}
	.merchant-sales-volume .Delivery{
		font-size:12px;
		float:right;
		color:white;
		background-color:#009BFF;
		border-radius:2px;
		padding:2px;
	}
	.Distribution-fee{
		margin-top:5px;
	}
	.Varieties{
		font-size:12px;
		border:1px solid #EEEEEE;
	}
</style>