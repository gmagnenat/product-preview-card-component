<script setup>
import ProductPreviewCard from './components/ProductPreviewCard.vue';
</script>

<template>
	<ProductPreviewCard />
</template>

<style>
:root {
	--color-green: #0a3e0a;
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
	font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
		Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
	box-sizing: border-box;
}

p {
	margin-bottom: 1rem;
}
</style>
