<template>
	<ul class="social-list">
		<a
			v-for="(item, index) in list"
			:key="index"
			class="social-item"
			:href="item.linkUrl">
			<SocialItem
				:imgUrl="require(`@/static/${item.imgUrl}`)"
			/>
		</a>
	</ul>
</template>

<script>
export default {
	data() {
		return {
			list: [
				{
					imgUrl: 'vk.svg',
					linkUrl: 'https://vk.com'
				},
				{
					imgUrl: 'inst.svg',
					linkUrl: 'https://github.com/daywalker0?tab=repositories'
				},
				{
					imgUrl: 'discord.svg',
					linkUrl: 'https://discord.com/'
				},
				{
					imgUrl: 'vector.svg',
					linkUrl: 'https://github.com/daywalker0?tab=repositories'
				},
				{
					imgUrl: 'mail.svg',
					linkUrl: 'https://mail.yandex.ru'
				},
			]
		}
	}
}
</script>

<style lang="scss" scoped>
.social-list {
	display: flex;
	gap: 15px;
}
</style>