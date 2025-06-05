<script setup lang="ts">

import HeartIcon from './icons/HeartIcon.vue';

const { score = 0 } = defineProps({ score: Number });

</script>

<template>
	<div class="score">{{ score }}<HeartIcon /></div>
</template>

<style scoped>
	.score {
		display: flex;
		flex-wrap: nowrap;
		align-items: center;
		gap: 10px;
		color: var(--color-primary);
		background-color: var(--color-secondary);
		border-radius: 30px;
		height: 48px;
		padding: 12px 24px;
	}
	.score svg {
		color: var(--color-primary);
	}

</style>