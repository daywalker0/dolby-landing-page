<template>
	<section class="s-recent">
		<div class="recent__container">
			<div class="recent__header">
				<h1 class="recent__title title">Recent Activity</h1>
				<NuxtLink to="" class="btn btn-browse-more-2">Browse More</NuxtLink>
			</div>
			<RecentSlider />
		</div>
	</section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.s-recent {
}
.recent {
	&__container {
		padding: 125px 0 106px;
	}
	&__header {
		display: flex;
		justify-content: space-between;
		padding-bottom: 27px;
	}
	&__title {
		font-size: 36px;
		line-height: 62px;
	}
}
.btn-browse-more-2 {
	padding-right: 120px;
	align-self: flex-end;
}

</style>