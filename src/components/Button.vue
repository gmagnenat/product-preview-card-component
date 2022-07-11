<template>
	<button class="btn">
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
.btn {
	background-color: var(--color-primary);
	color: #fff;
	border: none;
	padding: 1.2rem 1rem;
	width: 100%;
	height: 4.8rem;
	border-radius: 8px;
	font-size: 1.4rem;
	font-weight: 600;
	cursor: pointer;

	display: flex;
	flex-direction: row;
	justify-content: center;
	align-items: center;

	margin-top: 2rem;

	transition: all 0.2s ease-in-out;
}

.btn img {
	width: 16px;
	height: 16px;
	object-fit: contain;
	margin-right: 1rem;
}

.btn:hover {
	background-color: var(--color-deep-aquamarine);
}

@media screen and (min-width: 650px) {
	.btn {
		margin-top: 2.9rem;
	}
}
</style>
