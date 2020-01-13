<template>
 <div>
 	11115633332222323323
 	<childOne></childOne>
 	{{arr}}
 	<button @click="ccc">变化1</button>
 	<input type="text" v-model.lazy='message'/>
 	<div>{{message}}</div>
 	<div>
 		-----------------------------------------------------------------
 		<br /><br />
 		<big></big>
 	</div>
 </div>
 
</template>

<script>
	import big from './big'
	import childOne from './childOne'
	const cityOptions=['上海1', '北京', '广州', '深圳']
	
export default {
  name: 'HelloWorld',
 
  provide:{
  	for:'liwei啊啊啊'
  },
  
  components:{
  	childOne,
  	big
  },
  data(){
  	return {
  		arr:[2],
  		message:';oooo'
  	}
  },
  mounted(){
  	
  },
  methods:{
  	ccc:function(){
  		this.arr.length=4
  		this.arr.fill(1)
  		
  		console.log(this.arr)
  	}
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.my-autocomplete {
  li {
    line-height: normal;
    padding: 7px;

    .name {
      text-overflow: ellipsis;
      overflow: hidden;
    }
    .addr {
      font-size: 12px;
      color: #b4b4b4;
    }

    .highlighted .addr {
      color: #ddd;
    }
  }
}
	.wlselect{
		width:130px;
	}
	 .el-select .el-input {
    width: 130px;
  }
  .input-with-select .el-input-group__prepend {
    background-color: #fff;
  }
	.hello{
		margin-left:400px;
		margin-bottom:100px;
	}
	.el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
   .el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }
  
  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
  }
  
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
  
  body > .el-container {
    margin-bottom: 40px;
  }
  
  .el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }
  
  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }
</style>
