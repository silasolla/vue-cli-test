<template>
	<div>
		<p>{{ greet }}</p>
		<p>child_num: {{ child_num }}</p>
		<button @click='send'>親に値を渡す</button>
	</div>
</template>

<script>
	export default {
		props: {
			greet: {
				type: String,
				default: 'hogehoge'
			}
		},
		data: function(){
			return{
				child_num: 0
			};
		},
		methods: {
			send() {
				this.$emit("my-click", this.child_num);
			}
		}
	};
</script>
