<template>
	<div class="category">
		<h1>{{ title }}</h1>
	</div>
</template>

<script>
export default {
	name: "Category",
	props: {
		title: String,
		item: Object
	}
}
</script>

<style >
.category {
	width: 300px;
	float: left;
	display: block;
	background-color: #7A98EF;
	margin: 10px;
	min-height: 500px;
}
</style>