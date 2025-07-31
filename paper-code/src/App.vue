<template>
	<div class="container m-auto">
		<div class="title text-center mt-6 font-blod">
			<p class="text-5xl my-2 leading-12">Code as Policies:</p>
			<p class="text-xl">Language Model Programs for Embodied Control</p>
		</div>
		<AuthorInfo />
		<AbstractComp />
		<CodeBox :json="json1" />
	</div>
</template>

<script setup>
import AuthorInfo from './components/AuthorInfo.vue'
import AbstractComp from './components/AbstractComp.vue'
import CodeBox from './components/CodeBox.vue'
import json1 from './videoData.json'
console.log(json1)
</script>

<style scoped>
.container {
	width: 100%;
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #212529;
}

@media (min-width: 992px) {
	.container {
		max-width: 960px;
	}
}

@media (min-width: 768px) {
	.container {
		max-width: 720px;
	}
}

@media (min-width: 576px) {
	.container {
		max-width: 540px;
	}
}
</style>
