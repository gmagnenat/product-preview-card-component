<template>
	<div class="previewCard">
		<div class="previewCard-col">
			<p class="previewCard-subheading">Perfume</p>
			<h1 class="previewCard-heading">
				Gabrielle<br />
				Essence Eau De<br />
				Parfum
			</h1>
			<p class="previewCard-body">
				A floral, solar and voluptuous interpretation composed by Olivier Polge,
				Parfumer-Creator for the House of CHANEL
			</p>
			<div class="previewCard-price">
				<p class="previewCard-price-actual">$149.99</p>
				<p class="previewCard-price-original dashed">$169.99</p>
			</div>
			<Button class="previewCard-button" />
		</div>
		<div class="previewCard-col">
			<picture>
				<source
					class="previewCard-image"
					media="(max-width: 374px)"
					srcset="../assets/image-product-mobile.jpg"
				/>
				<source
					class="previewCard-image"
					media="(min-width: 375px)"
					srcset="../assets/image-product-desktop.jpg"
				/>
				<img
					class="previewCard-image"
					src="../assets/image-product-desktop.jpg"
					alt="Channel Parfum Bottle"
				/>
			</picture>
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
	width: 320px;
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	background-color: #f5f5f5;
	border-radius: 10px;

	display: flex;
	flex-direction: column;

	color: var(--color-green);

	box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
}

.previewCard-col:first-of-type {
	padding: 2.4rem;

	align-items: center;
	justify-content: center;
	order: 1;
}

.previewCard-heading {
	margin-top: 1.2rem;
}

.previewCard-subheading {
	text-transform: uppercase;
	letter-spacing: 5px;
	font-size: 1.2rem;
}

.previewCard-body {
	margin-top: 1.6rem;
}

.previewCard-image {
	width: 100%;
	height: 100%;
	max-height: 240px;
	object-fit: cover;
	border-top-left-radius: 10px;
	border-top-right-radius: 10px;
}

.previewCard-price {
	display: flex;
	flex-direction: row;
	align-items: center;

	margin-top: 2.4rem;
}

.previewCard-price .previewCard-price-actual {
	font-family: var(--ff-heading);
	color: var(--color-primary);
	margin-right: 3.2rem;
}

.previewCard-price-actual {
	font-size: 3rem;
	font-weight: 600;
}

.dashed {
	text-decoration: line-through;
}

@media screen and (min-width: 375px) {
	.previewCard {
		width: 600px;
		display: grid;
		grid-template-columns: 1fr 1fr;
	}

	.previewCard-image {
		width: 100%;
		height: 100%;
		max-height: 100%;
		object-fit: cover;
		border-top-left-radius: 10px;
		border-top-right-radius: 0;
		border-bottom-left-radius: 10px;
	}

	.previewCard-col:first-of-type {
		padding: 3.2rem;

		align-items: center;
		justify-content: center;
		order: 1;
	}

	.previewCard-heading {
		margin-top: 1.8rem;
	}

	.previewCard-body {
		margin-top: 2.3rem;
	}

	.previewCard-price {
		margin-top: 3.3rem;
	}
}
</style>
