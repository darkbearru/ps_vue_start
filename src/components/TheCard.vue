<script setup lang="ts">

const { index, word } = defineProps({ index: Number, word: String });

const emit = defineEmits(['turnOn', 'changeStatus']);

const turnOn = () => emit('turnOn');
const changeStatus = () => emit('changeStatus');

</script>

<template>
	<div class="card">
		<div class="border">
			<div class="border-label">{{ index }}</div>
			<div class="word">{{ word }}</div>
			<div class="border-buttons">
				<div class="label">перевернуть</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.card {
	display: flex;
	justify-content: stretch;
	align-items: stretch;
	width: 250px;
	height: 376px;
	border-radius: 16px;
	padding: 19px;
	box-shadow: 0 0 16px 0 #0000001A;
}
.border {
	position: relative;
	display: flex;
	align-items: center;
	justify-content: center;
	width: 100%;
	border: 1px solid var(--color-secondary);
	border-radius: 12px;
}
.border-label {
	position: absolute;
	top: -8px;
	left: 16px;
	padding: 0 4px;
	color: var(--color-black);
	background-color: var(--color-primary-inverted);
	font-size: 14px;
	font-weight: 400;
}
.border-buttons {
	position: absolute;
	display: flex;
	justify-content: center;
	bottom: -8px;
	padding: 0 4px;
	background-color: var(--color-primary-inverted);
}
.label {
	font-size: 12px;
	font-weight: 700;
	letter-spacing: 3px;
	text-transform: uppercase;
}
.word {
	font-size: 18px;
	font-weight: 400;
}
</style>