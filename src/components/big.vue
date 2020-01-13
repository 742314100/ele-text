<template>
	<div>
		<div>big</div>
		{{com1}}
		<keep-alive>
			<componnet :is='com1'>
				<p slot-scope='item'>
					牛雪威
					{{item.text}}
				</p>
				<div slot='s1'>
					蓝旗班车1
				</div>
				<div slot='s2'>
					蓝旗班车2
				</div>
				<div slot='s3'>
					蓝旗班车3
				</div>
			</componnet>
			
		</keep-alive>
		<button @click='btn'>切换</button>
	</div>
</template>

<script>
	import small1 from './small1'
	import small2 from './small2'
	var a=1
	export default {
		name:'big',
		data(){
			return {
				com1:'small1',
			}
		},
		components:{
			small1,
			small2
		},
		methods:{
			 btn(){
			 	if(a%2==1){
			 		this.com1='small2'
			 		a++
			 	}else{
			 		this.com1='small1'
			 		a++
			 	}
				
			}
		}
	}
</script>

<style>
</style>