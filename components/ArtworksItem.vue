<template>
	<article class="card-item"
		>
		<div class="card-item__wrap">
			<img :src="imgUrl" class="card-item__img" />
			<div class="card-item-info">
				<h4 class="card-item-info__title">{{ title }}</h4>
				<p class="card-item-info__descr">{{ descr }}</p>
				<div class="card-item-info-price">
					<span class="card-item-info__price_price">Price</span>
					<span class="card-item-info__price">{{ price }}</span>
				</div>
				<div class="card-item-info-btns">
					<a @click.prevent="activeFav(id)" href="" class="favourite-btn"><img src="~static/favourite.svg" alt=""></a>
					<button class="buy-btn">BUY</button>
				</div>
			</div>
		</div>
	</article>
</template>

<script>
export default {
	props: ['id', 'imgUrl', 'title', 'descr', 'price'],
	methods: {
		activeFav: function(clickedFavouiriteId) {
			document.querySelector('.favourite-btn').classList.toggle('activeFav');
		}
	}
}
</script>

<style lang='scss' scoped>
.card-item {
	&__wrap {
		background: rgba(255, 255, 255, 0.2);
		border-radius: 0px 0px 8px 8px;
	}
	&__img {
	}
}
.activeFav {
	background: url('~static/favourite-2.svg');
	background-repeat: no-repeat;
}
.card-item-info-price {
	display: flex;
	justify-content: space-between;
	align-items: center;
}
.card-item-info-btns {
	display: flex;
	justify-content: space-between;
	padding-top: 24px;
}
.buy-btn {
	font-family: 'Montserrat';
	font-weight: 600;
	font-size: 18px;
	line-height: 22px;
	text-align: center;
	color: #000000;
	background: #FDC500;
	border-radius: 3px;
	border: none;
	padding: 5px 17px;
	cursor: pointer;
}
.card-item-info {
	padding: 14px 14px 11px 11px;
	&__title {
		font-family: JosefinSans;
		font-weight: 600;
		font-size: 18px;
		line-height: 18px;
		color: rgba(255, 255, 255, 0.75);
	}
	&__descr {
		font-family: JosefinSans;
		font-weight: 400;
		font-size: 12px;
		line-height: 12px;
		text-transform: capitalize;
		color: rgba(255, 255, 255, 0.6);
		padding: 12px 0 20px;
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
		&_price {
			font-family: Poppins;
			font-weight: 400;
			font-size: 12px;
			line-height: 18px;
			text-transform: capitalize;
			color: #FFFFFF;
		}
	}
}
h4 { 
	margin-block-start: 0px;
	margin-block-end: 0px;
	margin-inline-start: 0px;
	margin-inline-end: 0px;
	font-weight: bold;
}

</style>