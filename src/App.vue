<script setup>
import ProductPreviewCard from './components/ProductPreviewCard.vue';
</script>

<template>
	<ProductPreviewCard />
</template>

<style>
:root {
	--color-primary: hsl(158, 36%, 37%);
	--color-primary-cream: hsl(30, 38%, 92%);
	--color-deep-aquamarine: hsl(212, 21%, 14%);
	--color-autometal-saurus: hsl(228, 12%, 48%);
	--color-white: hsl(0, 0%, 100%);

	--fs-body: 1.4rem;
	--lh-body: 23px;
	--lh-heading: 32px;

	--ff-body: 'Montserrat', sans-serif;
	--ff-heading: 'Fraunces', serif;

	--fw-500: 500;
	--fw-700: 700;
}

*,
*:before,
*:after {
	margin: 0;
	padding: 0;
}

html {
	font-size: 62.5%;
	box-sizing: inherit;
}

body {
	font-family: var(--ff-body);
	color: var(--color-autometal-saurus);
	box-sizing: border-box;
	font-size: var(--fs-body);
	line-height: var(--lh-body);
	background-color: var(--color-primary-cream);
}

h1 {
	font-family: var(--ff-heading);
	color: var(--color-deep-aquamarine);
	font-weight: var(--fw-700);
	font-size: 3.2rem;
	line-height: var(--lh-heading);
	margin-bottom: 1rem;
}

p {
	margin-bottom: 1rem;
}
</style>
