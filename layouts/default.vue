<template>
	<div class="default-layout">
		<TheHeader />
		<nuxt />
		<TheFooter />
	</div>
</template>

<script>
export default {
}
</script>

<style lang="scss">
.default-layout {
	background: linear-gradient(108.13deg, #320000 1%, #0F0323 37.66%, #322204 72.27%, #000230 98.74%);
	min-height: 100vh;
	font-family: Poppins;
	font-weight: 600;
	font-size: 18px;
	line-height: 28px;
	color: rgba(255, 255, 255, 0.75);
	position: relative;
	display: flex;
	flex-direction: column;
	width: 100%;
	overflow: hidden;
}
</style>