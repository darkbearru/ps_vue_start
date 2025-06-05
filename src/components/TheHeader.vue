<script setup lang="ts">

import TheScore from './TheScore.vue';
</script>

<template>
	<header class="header">
		<h1>Запомни слово</h1>
		<TheScore></TheScore>
	</header>
</template>

<style scoped>
.header {
	display: flex;
	flex-wrap: nowrap;
	align-items: center;
	justify-content: space-between;
	height: 120px;
	padding: 0 66px;
}
h1 {
	font-size: 16px;
	font-weight: 700;
	text-transform: uppercase;
}

</style>