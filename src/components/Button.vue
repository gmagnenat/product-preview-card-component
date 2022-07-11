<template>
	<button class="previewCard-button">
		<img src="../assets/icon-cart.svg" alt="" />
		Add to Cart
	</button>
</template>

<script>
export default {
	setup() {
		return {};
	},
};
</script>

<style scoped>
.previewCard-button {
	background-color: var(--color-green);
	color: #fff;
	border: none;
	padding: 1.2rem 1rem;
	width: 100%;
	border-radius: 4px;
	font-size: 1rem;
	font-weight: 600;
	cursor: pointer;

	display: flex;
	flex-direction: row;
	justify-content: center;
	align-items: center;

	transition: all 0.2s ease-in-out;
}

.previewCard-button img {
	width: 10px;
	margin-right: 0.5rem;
}

.previewCard-button:hover {
	background-color: #ffb300;
}
</style>
