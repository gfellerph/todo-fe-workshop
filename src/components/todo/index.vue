<template>
	<div>
		<addtodo></addtodo>
		<filter></filter>
		<list v-bind:todos='todos'></list>  
	</div>
</template>

<script>
	import addtodo from "./addtodo";
	import filter from "./filter";
	import list from "./list";

	export default {
		data: function (){
			return {
				todos:["fix","fertig"],
				activeFilter:null
			}
		},
		components:{
			addtodo,
			filter,
			list
		}  
	}
</script>

<style>
	

</style>