<template>
	<div class="super-menber">
		<div class="super-menber-box weui-flex">
			<div class="super-img">
				<img src="../../assets/images/super.png" />
			</div>
			<div class="super-text" style="flex:1;">
				<h1>超级会员</h1><span>•每月领20元红包</span>
			</div>
			<div class="super-open">
				<a href="#">立即开通> </a>
			</div>
		</div>
	</div>
</template>

<script>
</script>

<style>
	.super-menber {
		width: 100%;
		height: 45px;
		padding: 10px;
		box-sizing: border-box;
		color: #644f1b;
	}
	
	.super-menber-box {
		background-image: -webkit-gradient(linear, left top, right top, from(#ffefc4), to(#f3dda0));
		background-image: -webkit-linear-gradient(left, #ffefc4, #f3dda0);
		background-image: linear-gradient(90deg, #ffefc4, #f3dda0);
		width: 100%;
		height: 40px;
		position: relative;
	}
	
	.super-img {
		width: 40px;
		height: 40px;
	}
	
	.super-img img {
		width: 20px;
		height: 20px;
		margin: 10px 15px 0px;
	}
	
	.super-text {
		line-height: 40px;
	}
	
	.super-text h1 {
		font-size: 16px;
		display: inline-block;
		margin-right: 3px;
	}
	
	.super-text span {
		font-size: 12px;
	}
	
	.super-open {
		width: 80px;
		height: 40px;
		text-align: center;
		line-height: 40px;
	}
	.super-open a{
		color:#644f1b;
		font-size:12px;
	}
</style>