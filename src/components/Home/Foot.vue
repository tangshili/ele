<template>
	<div class="foot">
		<ul>
			<li v-for="(item,index) in nav">
				<router-link :to="item.to">
					<span class="fa" :class="item.icon"></span>
					<span class="title" v-text="item.title"></span>
				</router-link>
			</li>
		</ul>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				nav: [{
					title: '首页',
					icon: 'fa-home',
					to:'/',
				},{
					title: '发现',
					icon: 'fa-refresh',
					to:'#',
				},{
					title: '订单',
					icon: 'fa-file-text-o',
					to:'#',
				},{
					title: '我的',
					icon: 'fa-user',
					to:'#',
				}]
			}
		}
	}
</script>

<style>
	.foot {
		width: 100%;
		height: 50px;
		position: fixed;
		bottom: 0px;
		left: 0px;
		text-align: center;
		z-index: 9999;
		background-color:white;
		box-shadow: 0px 0px 15px #ccc;
	}
	
	.foot ul li {
		width: 25%;
		float:left;
		text-align: center;
	}
	
	.foot ul li .title {
		font-size: 12px;
		line-height: 27px;
		color:#333333;	
	}
	
	.foot ul li .fa {
		font-size: 20px;
		line-height: 13px;
		display:block;
		color:#333333;
		margin-top:10px;
	}
	
	.foot ul li :hover span {
		color: #0085FF;
	}
</style>