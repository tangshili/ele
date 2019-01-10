<template>
	<div class="search-bar">
		<div class="position">
			<img src="../../assets/images/position.png" />
			<h1>蚂蚁创客小镇</h1>
			<select>
				<option></option>
			</select>
		</div>
		<div class="search">
			<i class="fa fa-search"></i>
			<input type="text" name="text" id="text" placeholder="搜索饿了么商家、商品名称……" />
		</div>
	</div>
</template>

<script>
	
</script>

<style>
	.search-bar {
		width: 100%;
		background-image: -webkit-gradient(linear, left top, right top, from(#0af), to(#0085ff));
		background-image: -webkit-linear-gradient(left, #0af, #0085ff);
		background-image: linear-gradient(90deg, #0af, #0085ff);
		height:105px;
		font-family: "微软雅黑";
	}
	
	.search-bar .position {
		width: 100%;
		padding: 20px;
		box-sizing: border-box;
		height: 45px;
	}
	
	.search-bar .position img {
		width: 20px;
		height: 20px;
		margin-right: 10px;
	}
	
	.search-bar .position h1 {
		font-size: 18px;
		color: white;
		display: inline-block;
		line-height: 20px;
		margin-right: 5px;
	}
	
	.search-bar .search {
		width: 100%;
		height: 60px;
		padding: 10px 20px;
		box-sizing: border-box;
		position: relative;
	}
	
	.search-bar .search input {
		width: 100%;
		height: 40px;
		border: 0px;
		padding-left: 70px;
		box-sizing: border-box;
		font-family: simsun;
	}
	
	.search-bar .search i.fa {
		position: absolute;
		top: 20px;
		left: 68px;
		color: #ccc;
	}
</style>