<template>
	<div class="w-10/12 sm:w-80 h-96 mx-auto bg-white rounded-md overflow-hidden shadow-sm">
		<img :src="getImage(this.image)" class="w-full h-1/2 object-cover" alt="">
		<slot></slot>
	</div>
</template>

<script>
	export default {
		props: ['img'],
		data() {
			return {
				image: this.img,
			}
		},
		methods: {
			getImage(img) {
				return require(`../assets/images/${img}`)
			}
		}
	}
</script>