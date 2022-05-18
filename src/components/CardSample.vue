<template>
	<div>
		<div class="blue-b mb-4">
			<p>id: {{ id }}</p>
			<p>title: {{ title }}</p>
			<p>image: {{ image }}</p>
			<p>description: {{ description }}</p>
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
		border: 1px solid blue;
	}
	.mb-4{
		margin: 4px;
		padding: 4px;
	}
</style>
