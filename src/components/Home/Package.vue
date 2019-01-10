<template>
	<div class="package weui-flex">
		<div class="quality">
			<div class="quality-title1">品质套餐</div>
			<div class="quality-title2">搭配齐全吃得好</div>
			<div class="quality-title3">立即购买></div>
			<div class="quality-img">
				<img src="../../assets/images/quality.png" />
			</div>
		</div>
		<div class="limited">
			<div class="limited-title1">限量换购</div>
			<div class="limited-title2">超值美味9.9元起</div>
			<div class="limited-title3"><span style="color:#e81919;">890人</span>正在抢></div>
			<div class="limited-img">
				<img src="../../assets/images/limited.png" />
			</div>
		</div>
	</div>
</template>

<script>
</script>

<style>
	.package {
		width: 100%;
		height: 170px;
		padding: 10px;
		box-sizing: border-box;
	}
	
	.package .quality {
		flex: 1;
		margin-right: 5px;
		padding: 10px;
		position: relative;
		background-color: #F8F8F8;
	}
	
	.package .limited {
		flex: 1;
		margin-left: 5px;
		padding: 10px;
		position: relative;
		background-color: #F8F8F8;
	}
	
	.package .quality-title1 {
		font-size: 16px;
		line-height: 28px;
		color: #333333;
	}
	
	.package .quality-title2 {
		font-size: 12px;
		color: #666;
		line-height: 20px;
	}
	
	.package .quality-title3 {
		font-size: 12px;
		color: #af8260;
		line-height: 20px;
	}
	
	.package .quality-img {
		width: 140px;
		height: 90px;
		position: absolute;
		bottom: 0px;
		right: 5px;
	}
	
	.package .quality-img img {
		width: 140px;
		height: 90px;
	}
	
	.package .limited-title1 {
		font-size: 16px;
		line-height: 28px;
		color: #e81919;
	}
	
	.package .limited-title2 {
		font-size: 12px;
		color: #666;
		line-height: 20px;
	}
	
	.package .limited-title3 {
		font-size: 12px;
		line-height: 20px;
		color: #333333;
	}
	
	.package .limited-img {
		width: 140px;
		height: 90px;
		position: absolute;
		bottom: 0px;
		right: 5px;
	}
	
	.package .limited-img img {
		width: 140px;
		height: 90px;
	}
</style>