<template>
	<div>
	<p>{{todos}}{{activeFilter}}
	<ul>
		<li v-for="todo in todos">
			<item v-bind:todo="todo"></item>
		</li>
	</ul>
	</div>
</template>

<script >
import item from "./item";

export default {
	props: {
		todos: Array
	},
	components:{
		item
	}

	
}
</script>