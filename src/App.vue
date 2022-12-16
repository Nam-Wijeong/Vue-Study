<template>
	<div class="menu">
		<a v-for="(menu, i) in menus" :key="i">{{ menu }}</a>
	</div>
	<div v-for="(product, i) in products" :key="i">
		<h4>{{ product }}</h4>
		<p>{{ price1 }} 만원</p>
	</div>
</template>

<script>
// 데이터 바인딩 하는 이유
// 1. HTML 하드코딩하면 나중에 변경이 어려움
// 2. 뷰의 실시간 자동 렌더링 기능 사용
export default {
	name: 'App',
	data() {
		return {
			menus: ['Home', 'Shop', 'About'],
			price1: 60,
			price2: 70,
			products: ['역삼동 원룸', '천호동 원룸', '마포구 원룸'],
		};
	},
	components: {},
};
</script>

<style></style>
