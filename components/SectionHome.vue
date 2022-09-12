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
		font-family: JosefinSans;
		font-weight: 700;
		font-size: 80px;
		line-height: 80px;
		letter-spacing: 0.1em;
		color: #FFFFFF;
		opacity: 0.75;
		text-transform: uppercase;
	}
	&__subtitle {
		font-size: 16px;
		font-weight: 400;
		line-height: 28px;
		letter-spacing: -0.02em;
		color: rgba(255, 255, 255, 0.75);
		padding: 25px 0 27px;
	}
}
.title {
}
.subtitle {
}
.btn {
	font-size: 18px;
	line-height: 28px;
	color: rgba(255, 255, 255, 0.75);
	text-decoration: none;
	&::after {
		content: '';
		background: url('~static/arrow.svg');
		background-size: cover;
		height: 20px;
		width: 45px;
		display: inline-block;
		margin-left: 12px;
		vertical-align: middle;
	}
}
.btn-get-started {
}
.home-defi-image {
}
</style>