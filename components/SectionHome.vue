<template>
	<section class="s-home">
		<div class="home__container">
			<div class="home-content">
				<p class="home-content__text">Featured Film</p><br>
				<h1 class="home-content__title title">zero<br>contact</h1><br>
				<h3 class="home-content__subtitle subtitle">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit<br>gravida enim, orci morbi elementum gravida. </h3>
				<NuxtLink to="" class="btn btn-get-started">Let's get started</NuxtLink>
				<HomeBlockList />
			</div>
			<div class="home-defi-image">
				<img src="~static/defi.png" alt="">
			</div>
		</div>
	</section>
</template>

<script>
export default {
	data() {
		return {
		}
	}
}
</script>

<style lang="scss" scoped>
.s-home {
}
.home {
	&__container {
		display: flex;
		justify-content: space-between;
		position: relative;
		padding: 140px 0 180px;
	}
}
.home-content {
	&__text {
		font-family: JosefinSans;
		font-weight: 600;
		font-size: 24px;
		line-height: 33px;
		letter-spacing: 0.1em;
		color: #FFFFFF;
	}
	&__title {
		font-size: 80px;
		line-height: 80px;
		text-transform: uppercase;
		letter-spacing: 0.1em;
	}
	&__subtitle {
		font-size: 16px;
		letter-spacing: -0.02em;
		color: rgba(255, 255, 255, 0.75);
		padding: 0 0 27px;
	}
}
.btn-get-started {
}
.home-defi-image {
	position: absolute;
	right: -75px;
	top: -40px;
	background: rgba(255, 255, 255, 0.1);
	border-radius: 330px;
	img {
		padding: 70px 40px;
	}
}
</style>