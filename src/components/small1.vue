<template>
	<div>
		{{aa}}
		<button @click='bian'>bbbbbb</button>
		<slot text='哦哦哦哦哦'></slot>
		<slot name='s1'></slot>
		<slot name='s2'></slot>
		<slot name='s3'></slot>
	</div>
</template>

<script>
	export default {
		name:'small1',
		data(){
			return {
				aa:'small1'
			}
		},
		methods:{
			bian(){
				this.aa='smallllllllll'
			}
		}
	}
</script>

<style>
</style>