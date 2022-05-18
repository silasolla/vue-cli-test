<template>
	<div class="red-b flex-container">
		<div v-for="card of cards" :key="card">
			<CardSample :id="card.id" :title="card.title" :image="card.image" :description="card.description"/>
		</div>
	</div>
</template>

<script>
	import CardSample from '@/components/CardSample'
	export default {
		name: 'App',
		components: {
			CardSample
		},
		data(){
			return{
				cards: [
					{
						id: 1,
						title: 'タイトル1',
						image: 'img1.jpg',
						description: '詳細1'	
					},
					{
						id: 2,
						title: 'タイトル2',
						image: 'img2.jpg',
						description: '詳細2'	
					},
					{
						id: 3,
						title: 'タイトル3',
						image: 'img3.jpg',
						description: '詳細3'	
					}
				]
			}
		}
	}
</script>

<style scoped>
	.red-b{
		border: 1.5px solid red;
	}
	.flex-container {
		display: flex;
		justify-content: space-around; 
	}
</style>
