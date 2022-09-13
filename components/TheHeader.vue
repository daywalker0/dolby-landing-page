<template>
	<header class="header">
		<div class="header__logo"><span>d</span>olby.</div>
		<div class="header__container">
		</div>
	</header>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.header {
	z-index: 50;
	display: flex;
	&__container {
		min-height: 100px;
	}
	&__logo {
		font-family: JosefinSans;
		font-size: 36px;
		font-weight: 700;
		color: #FFFFFF;
		align-self: flex-end;
		padding: 0 0 13px 50px;
		span {
			color: #FEDB62;
		}
	}
}
@media (min-width: 1650px) {
	.header__logo {
		padding-left: 200px;
	}
}
</style>