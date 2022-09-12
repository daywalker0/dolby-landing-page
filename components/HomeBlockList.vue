<template>
	<div class="home-content__info-blocks">
		<div
			v-for="(block, index) in blocks"
			:key="index"
			class="block-item"> {{ block.quantity }} | {{ block.info }}
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			blocks: [
				{
					quantity: '2k',
					info: 'Active user'
				},
				{
					quantity: '5k',
					info: 'Music Video'
				},
				{
					quantity: '7k',
					info: 'Visual Art'
				},
			]
		}
	},
}
</script>

<style lang="scss" scoped>
.home-content__info-blocks {
	padding-top: 68px;
	display: flex;
	gap: 45px;
}

</style>