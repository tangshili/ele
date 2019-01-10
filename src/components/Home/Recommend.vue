<template>
	<div class="recommend">
		<div class="recommend-title">→&nbsp;&nbsp;推荐商家&nbsp;&nbsp;←</div>
		<div class="recommend-list weui-flex">
			<div class="recommend-list1" style="flex: 1;">综合排序
				<svg style="width:10px;" data-v-a5cc4024="" viewBox="0 0 72 32" class="dropdown-icon">
					<path data-v-a5cc4024="" d="M36 32l36-32h-72z"></path>
				</svg>
			</div>
			<div class="recommend-list2" style="flex: 1;">距离最近</div>
			<div class="recommend-list3" style="flex: 1;">品质联盟</div>
			<div class="recommend-list4" style="flex: 1;">筛选  <img style="width:12px;" src="../../assets/images/filter.png"/></div>
		</div>
	</div>
</template>

<script>
</script>

<style>
	.recommend {
		width: 100%;
		height: 80px;
		padding: 0px 10px;
		box-sizing: border-box;
		color:#333333;
		border-bottom:1px solid #DDDDDD;		
	}
	
	.recommend .recommend-title {
		width: 100%;
		height: 40px;
		text-align: center;
		line-height: 50px;
		font-size:16px;
	}
	
	.recommend .recommend-list {
		width: 100%;
		height: 40px;
		text-align: center;
		line-height:40px;
		font-size:14px;
	}
</style>