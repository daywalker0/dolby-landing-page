<template>
	<div class="social-item__wrap">
		<a href="linkUrl" target="_blank">
			<img :src="imgUrl" alt="">
		</a>
	</div>
</template>

<script>
export default {
	props: [
		'imgUrl'
	]
}
</script>

<style lang="scss" scoped>
.social-item {
	&__wrap {
		background: rgba(255, 255, 255, 0.35);
		border-radius: 4px;
		width: 55px;
		height: 55px;
		text-align: center;
		img {
			transform: translateY(80%);
		}
	}
}
</style>