<template>
	<div class="swiper-container">
		<div class="swiper-wrapper">
			<div class="swiper-slide">
				<a href="#"><img src="../../assets/images/swiper-1.png"></a>
			</div>
			<div class="swiper-slide">
				<a href="#"><img src="../../assets/images/swiper-2.png"></a>
			</div>
			<div class="swiper-slide">
				<a href="#"><img src="../../assets/images/swiper-3.png"></a>
			</div>
		</div>
		<div class="swiper-pagination"></div>
	</div>
</template>

<script>
	import Swiper from "swiper"
	import "swiper/dist/css/swiper.min.css"
	export default {
		mounted: function() {
			var swiper = new Swiper('.swiper-container', {
				spaceBetween: 0,
				centeredSlides: true,
				autoplay: {
					delay: 2500,
					disableOnInteraction: false,
				},
				pagination: {
					el: '.swiper-container .swiper-pagination',
					clickable: true,
				}
			});
		}
	}
</script>

<style>
	.swiper-wrapper a {
		display: block;
		width: 100%;
	}
	
	.swiper-wrapper a img {
		width: 95%;
		margin: 0px 10px;
	}
</style>