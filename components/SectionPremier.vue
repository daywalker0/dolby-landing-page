<template>
	<section class="s-premier">
		<div class="premier__container">
			<h1 class="premier__title title">The Premier Marketplace<br>
for Nifties</h1>
			<p class="premier__subtitle subtitle">dolby is the premier marketplace for Nifties,
				which are digital items you can truly own. Digital Items have existed for a long time, but never like this.</p>
			<NuxtLink to="" class="btn btn-get-started-2">Let's get started</NuxtLink>
			<div class="premier__img-1"><img src="~static/blockchain.png" alt=""></div>
			<div class="premier__img-2"><img src="~static/central-bank.png" alt=""></div>
			<div class="premier__img-3"><img src="~static/yellow-boy.png" alt=""></div>
		</div>
	</section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.s-premier {
	background: rgba(255, 255, 255, 0.07);
}
.premier {
		&__container {
			position: relative;
			padding-bottom: 333px;
		}
		&__title {
			font-size: 48px;
			padding: 188px 0 33px;
			line-height: 62px;
		}
		&__subtitle {
			font-size: 18px;
			padding-bottom: 68px;
			max-width: 480px;
		}
		&__img-1 {
			position: absolute;
			right: 0;
			top: 88px;
			background: #94EEE5;
			border-radius: 50%;
			padding: 25px;
		}
		&__img-2 {
			position: absolute;
			right: 40%;
			bottom: 15%;
			background: #E87993;
			border-radius: 50%;
		}
		&__img-3 {
			position: absolute;
			right: 26%;
			bottom: 7%;
		}
}
.btn-get-started-2 {
	margin-left: 13px;
}

</style>