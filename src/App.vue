<template>
	<div>
		<h1>Hello from App.vue</h1>
		<!-- 挙動がよくわからん(上書きできない??)
		<ChildSample greet='Hello with props'/>
		-->
		<p>parent_num: {{ parent_num }}</p>
		<ChildSample @my-click='parent_num = $event'/>
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
