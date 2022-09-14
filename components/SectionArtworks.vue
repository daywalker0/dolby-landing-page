<template>
	<section class="s-artworks">
		<div class="artworks__container">
			<div class="artworks__header">
				<h2 class="artworks__title title">Features Artworks</h2>
				<NuxtLink to="" class="btn btn-browse-more">Browse More</NuxtLink>
			</div>
			<ArtworksSlider />
		</div>
	</section>
</template>

<script>
export default {
	name: 'IndexPage',
}
</script>

<style lang="scss" scoped>
.s-artworks {
	padding-bottom: 128px;
}
.artworks {
	&__title {
		font-size: 36px;
		line-height: 62px;
	}
	&__container {
	}
	&__header {
		display: flex;
		justify-content: space-between;
		padding-bottom: 27px;
	}
}
.btn-browse-more {
	align-self: flex-end;
	padding-right: 143px;
}
</style>