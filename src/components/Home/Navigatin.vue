<template>
	<div class="navigatin clear">
		<div class="navigatin-box">
			<div class="navigatin-text" v-for="(item,index) in arr">
				<roter-link :to="item.to">
					<img :src="item.image" />
					<div v-text="item.title"></div>
				</roter-link>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				arr: [{
					title: '美食',
					image: require('../../assets/images/food.png'),
					to: '#'
				},{
					title: '午餐',
					image: require('../../assets/images/lunch.png'),
					to: '#'
				},{
					title: '商超便利店',
					image: require('../../assets/images/convenience.png'),
					to: '#'
				},{
					title: '水果',
					image: require('../../assets/images/fruit.png'),
					to: '#'
				},{
					title: '医药健康',
					image: require('../../assets/images/medicine.png'),
					to: '#'
				},{
					title: '鲜花绿植',
					image: require('../../assets/images/flowers.png'),
					to: '#'
				},{
					title: '厨房生鲜',
					image: require('../../assets/images/kitchen.png'),
					to: '#'
				},{
					title: '跑腿代购',
					image: require('../../assets/images/run-leg.png'),
					to: '#'
				},{
					title: '甜品饮品',
					image: require('../../assets/images/dessert.png'),
					to: '#'
				},{
					title: '签到领红包',
					image: require('../../assets/images/envelop.png'),
					to: '#'
				}]
			};
		}
	}
</script>

<style>
	.clear:after{
		display:block;
		content: "";
		clear:both;
	}
	.navigatin {
		font-size:12px;
	}
	.navigatin .navigatin-box {
		text-align: center;
		margin-top: 10px;
	}
	
	.navigatin .navigatin-box .navigatin-text {
		float: left;
		width: 20%;
		margin-bottom: 15px;
	}
	
	.navigatin .navigatin-box .navigatin-text img {
		width: 50px;
		height: 50px;
		margin-bottom: 5px;
	}
	
	.navigatin a {
		display: block;
		text-decoration: none;
		color: #333;
		font-size: 14px;
	}
</style>