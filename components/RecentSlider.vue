<template>
	<div class="recent-slider">
		<div class="swiper-buttons">
			<div ref="prev" class="swiper-button-prev"></div>
			<div ref="next" class="swiper-button-next"></div>
		</div>
		<swiper
      :slides-per-view="3"
      :space-between="31"
      :loop="false"
			:navigation="{
				prevEl: prev,
				nextEl: next,
    	}"
    >
			<swiper-slide
				v-for="(card, index) in cards"
				:key="index">
				<RecentItem
				:title="card.title"
				:price="card.price"
				:imgUrl="require(`~/static/${card.imgUrl}`)" />
			</swiper-slide>
    </swiper>
	</div>
</template>

<script>
import { ref } from 'vue';
import { Navigation } from 'swiper'
import { SwiperCore, Swiper, SwiperSlide } from 'swiper-vue2'
import 'swiper/swiper-bundle.css'
SwiperCore.use([Navigation])
export default {
	data() { 
    return {
      cards: [
				{
					id: 1,
					imgUrl: "recent-img-1.png",
					title: 'Keeping yourself safe when buying NFTs on dolbi',
					price: '€25.00',
				},
				{
					id: 2,
					imgUrl: "recent-img-2.png",
					title: 'Keeping yourself safe when buying NFTs on dolbi',
					price: '€25.00',
				},
				{
					id: 3,
					imgUrl: "recent-img-3.png",
					title: 'Keeping yourself safe when buying NFTs on dolbi',
					price: '€25.00',
				},
				{
					id: 4,
					imgUrl: "recent-img-3.png",
					title: 'Keeping yourself safe when buying NFTs on dolbi',
					price: '€25.00',
				},
      ]
    }
	},
	 components: {
    Swiper,
    SwiperSlide
  },
	  setup() {
    const prev = ref(null);
    const next = ref(null);
    return {
      modules: [Navigation],
      prev,
      next,
    };
  }
}
</script>

<style lang="scss">
.recent-slider {
	position: relative;
}
.swiper-buttons {
	position: absolute;
	right: 0;
	top: -40px;
}
.swiper-button-prev {
	position: absolute;
	color: rgba(255, 255, 255, 0.75);
	left: -67px;
	&::after {
		font-size: 21px;
	}
}
.swiper-button-next {
	position: absolute;
	color: rgba(255, 255, 255, 0.75);
	right: 0px;
	&::after {
		font-size: 21px;
	}
}
</style>