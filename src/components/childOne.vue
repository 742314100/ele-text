<template>
	<div>
		{{demo}}
		<childtwo></childtwo>
	</div>
</template>

<script>
	import childtwo from './ChildTwo'
	export default {
		name:'childOne',
		inject:['for'],
		data(){
			return {
				demo:this.for
			}
		},
		components:{
			childtwo
		}
	}
</script>

<style>
</style>