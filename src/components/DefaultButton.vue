<script setup lang="ts">

const { color = 'var(--color-primary)' } = defineProps({ color: String });
</script>

<template>
	<button class="default-button" :style="{ backgroundColor: color }">
		<slot />
	</button>
</template>

<style scoped>
.default-button {
	display: flex;
	align-items: center;
	justify-content: center;
	min-width: 300px;
	height: 68px;
	border: none;
	border-radius: 100px;
	color: var(--color-primary-inverted);
	font-size: 24px;
	cursor: pointer;
}
</style>