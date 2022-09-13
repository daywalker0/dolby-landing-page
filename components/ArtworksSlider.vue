<template>
	<div class="artworks-slider">
		<div class="swiper-buttons">
			<div class="swiper-button-prev"></div>
			<div class="swiper-button-next"></div>
		</div>
		<div class="swiper mySwiper">
			<div class="swiper-wrapper">
				<div
					class="swiper-slide card"
					v-for="(card, index) in cards"
					:key="index">
				<ArtworksItem
					:title="card.title"
					:price="card.price"
					:descr="card.descr"
					:imgUrl="require(`~/static/${card.imgUrl}`)"
				/>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import { Swiper, Navigation} from 'swiper';
import 'swiper/swiper-bundle.min.css'
export default {
	mounted() {
		const swiper = new Swiper('.swiper', {
			modules: [Navigation],
			navigation: {
				nextEl: '.swiper-button-next',
				prevEl: '.swiper-button-prev',
			},
			slidesPerView: 4,
			loop: true,
			spaceBetween: 34,
		})
	},
	data() {
    return {
      cards: [
				{
					id: 1,
					imgUrl: "card-image-1.png",
					title: 'Jenuine Ruddy Girl',
					descr: 'Till Lindemann by NFT Frame Art',
					price: '€25.00',
				},
				{
					id: 2,
					imgUrl: "card-image-2.png",
					title: 'Jenuine Ruddy Girl',
					descr: 'Till Lindemann by NFT Frame Art',
					price: '€25.00',
				},
				{
					id: 3,
					imgUrl: "card-image-3.png",
					title: 'Jenuine Ruddy Girl',
					descr: 'Till Lindemann by NFT Frame Art',
					price: '€25.00',
				},
				{
					id: 4,
					imgUrl: "card-image-4.png",
					title: 'Jenuine Ruddy Girl',
					descr: 'Till Lindemann by NFT Frame Art',
					price: '€25.00',
				},
				{
					id: 5,
					imgUrl: "card-image-5.png",
					title: 'Jenuine Ruddy Girl',
					descr: 'Till Lindemann by NFT Frame Art',
					price: '€25.00',
				},

      ]
    }
	},
}
</script>

<style lang="scss" scoped>
.artworks-slider {
	position: relative;
}
.swiper-buttons {
	position: absolute;
	right: 40px;
	top: -40px;
}
.swiper-button-prev {
	position: absolute;
	left: -37px;
	color: rgba(255, 255, 255, 0.75);
	&::after {
		font-size: 21px;
	}
}
.swiper-button-next {
	position: absolute;
	right: -37px;
	color: rgba(255, 255, 255, 0.75);
	&::after {
		font-size: 21px;
	}
}
</style>