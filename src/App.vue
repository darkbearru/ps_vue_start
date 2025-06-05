<script setup>
import DefaultButton from "./components/DefaultButton.vue";
import TheHeader from "./components/TheHeader.vue";
import TheCard from "./components/TheCard.vue";
</script>

<template>
	<TheHeader></TheHeader>
	<main>
		<DefaultButton color="#008BFE">
			Начать игру
		</DefaultButton>
		<TheCard word="Hello" index="01"></TheCard>
	</main>
</template>

<style scoped>
	main {
		display: grid;
		place-items: center;
		min-height: 100vh;
	}
</style>
