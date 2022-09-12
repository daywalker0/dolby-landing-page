<template>
	<footer class="footer">
		<div class="footer__container">
			<div class="footer__left-content">
				<h2 class="footer__title">Join the community</h2>
				<SocialList />
			</div>
		</div>
	</footer>
</template>

<script>
export default {
}
</script>

<style lang="scss">
.footer {
	border-top: 1px solid #958F8F;
		&__container {
			display: grid;
			grid-template-columns: 44.65% 55.35%;
			gap: 50px;
			padding-bottom: 65px;
			padding-top: 73px;
		}
		&__left-content {
		}
		&__title {
			font-size: 24px;
			line-height: 36px;
			text-transform: capitalize;
			color: #FFFFFF;
			padding-bottom: 26px;
		}
		&__right-content {
		}
}
.title {
}

</style>