<template>
	<div>
		<h1>Hello from App.vue</h1>
		<p>parent_num: {{ parent_num }}</p>
		<ChildSample greet='Hello with props' @my-click='parent_num = $event'/>
	</div>
</template>

<script>
	import ChildSample from './components/ChildSample.vue'
	export default {
		name: 'App',
		components: {
			ChildSample
		},
		data(){
			return{
				parent_num: 100
			}
		}
	}
</script>
