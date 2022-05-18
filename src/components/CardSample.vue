<template>
	<div>
		<div class="blue-b mp-4">
			id: <div class="emph">{{ id }}</div><br>
			title: <div class="emph">{{ title }}</div><br>
			image: <div class="emph">{{ image }}</div><br>
			description: <div class="emph">{{ description }}</div>
		</div>
	</div>
</template>

<script>
	export default {
		props: {
			id: Number,
			title: String,
			image: String,
			description: String
		}
	}
</script>

<style scoped>
	.blue-b{
		border: 1.5px solid blue;
	}
	.mp-4{
		margin: 4px;
		padding: 4px;
	}
	.emph{
		font-weight: bold;
		color: fuchsia;
		display: inline;
	}
</style>
