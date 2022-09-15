<template>
	<article class="recent-card-item"
		>
		<div class="recent-card-item__wrap">
			<img :src="imgUrl" class="recent-card-item__img" />
			<div class="recent-card-item-info">
				<h4 class="recent-card-item-info__title">{{ title }}</h4>
				<span class="recent-card-item-info__price">{{ price }}</span>
			</div>
		</div>
	</article>
</template>

<script>
export default {
	props: ['id', 'imgUrl', 'title', 'price'],
}
</script>

<style lang='scss' scoped>
.recent-card-item {
	&__wrap {
	}
	&__img {
	}
}
.recent-card-item-info {
	&__title {
		font-family: JosefinSans;
		font-weight: 600;
		font-size: 18px;
		line-height: 28px;
		color: rgba(255, 255, 255, 0.75);
		padding: 22px 0 15px;
	}
	&__price {
		font-family: Poppins;
		font-weight: 600;
		font-size: 16px;
		line-height: 24px;
		color: #FFFFFF;
		&::before {
			content: '';
			background: url('~static/eth.svg');
			background-size: cover;
			height: 24px;
			width: 15px;
			display: inline-block;
			margin-right: 5px;
			vertical-align: middle;
		}
	}
}

</style>