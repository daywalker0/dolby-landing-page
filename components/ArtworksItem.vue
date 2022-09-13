<template>
	<article class="card-item"
		>
		<div class="card-item__wrap">
			<img :src="imgUrl" class="card-item__img" />
			<div class="card-item-info">
				<h4 class="card-item-info__title">{{ title }}</h4>
				<p class="card-item-info__descr">{{ descr }}</p>
				<span class="card-item-info__price">{{ price }}руб.</span>
			</div>
		</div>
	</article>
</template>

<script>
export default {
	props: ['imgUrl', 'title', 'descr', 'price']
}
</script>

<style>

</style>