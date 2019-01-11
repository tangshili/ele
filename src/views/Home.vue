<template>
	<div class="home">
		<search-bar></search-bar>
		<navigatin></navigatin>
		<super-member></super-member>
		<package></package>
		<swiper></swiper>
		<recommend></recommend>
		<merchant></merchant>
		<foot></foot>

	</div>

</template>

<script>
	// @ is an alias to /src
	import searchBar from '@/components/Home/searchBar.vue'
	import Navigatin from '@/components/Home/Navigatin.vue'
	import SuperMember from '@/components/Home/SuperMember.vue'
	import Package from '@/components/Home/Package.vue'
	import Swiper from '@/components/Home/Swiper.vue'
	import Recommend from '@/components/Home/Recommend.vue'
	import Merchant from '@/components/Home/Merchant.vue'
	import Foot from '@/components/Home/Foot.vue'


	export default {
		name: 'home',
		components: {
			searchBar,
			Navigatin,
			SuperMember,
			Package,
			Swiper,
			Recommend,
			Merchant,
			Foot
			
		}
	}
</script>