<script setup>
import DefaultButton from "./components/DefaultButton.vue";
</script>

<template>
	<main>
		<DefaultButton color="#008BFE">
			Начать игру
		</DefaultButton>
	</main>
</template>

<style scoped>
	main {
		display: grid;
		place-items: center;
		min-height: 100vh;
	}
</style>
