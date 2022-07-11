<template>
	<div class="previewCard">
		<div class="previewCard-col">
			<p>Perfume</p>
			<h1>Gabrielle Essence Eau De Parfum</h1>
			<p>
				A floral, solar and voluptuous interpretation composed by Oliver Polge,
				Parfumer-Creator for the House of CHANEL
			</p>
			<div class="previewCard-price">
				<p class="previewCard-price-actual">$100</p>
				<p class="previewCard-price-original dashed">$200</p>
			</div>
			<Button />
		</div>
		<div class="previewCard-col">
			<img
				class="previewCard-image"
				src="../assets/image-product-desktop.jpg"
				alt=""
			/>
		</div>
	</div>
</template>

<script>
import Button from './Button.vue';
export default {
	setup() {
		return {};
	},
	components: {
		Button,
	},
};
</script>

<style scoped>
.previewCard {
	max-width: 600px;
	position: absolute;
	top: 45%;
	left: 50%;
	transform: translate(-50%, -50%);
	background-color: #f5f5f5;
	border-radius: 4px;

	color: var(--color-green);

	display: grid;
	grid-template-columns: 1fr 1fr;

	box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
}

.previewCard-col:first-of-type {
	padding: 2rem;

	align-items: center;
	justify-content: center;
	order: 1;
}

.previewCard h1 {
	font-size: 1.5rem;
	font-weight: 500;
	margin-bottom: 1rem;
}

.previewCard-image {
	width: 100%;
	height: auto;
	object-fit: cover;
	border-top-left-radius: 10px;
	border-bottom-left-radius: 10px;
}

.previewCard-price {
	display: flex;
	flex-direction: row;
	align-items: center;
}

.previewCard-price .previewCard-price-actual {
	margin-right: 1rem;
}

.previewCard-price-actual {
	font-size: 3rem;
	font-weight: 600;
}

.dashed {
	text-decoration: line-through;
}
</style>
