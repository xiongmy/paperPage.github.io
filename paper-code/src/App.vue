<template>
	<div class="container m-auto">
		<div class="title text-center mt-10">
			<p class="my-2 leading-12" style="font-weight: bolder; font-size: 2.6rem;">Code as Policies:</p>
			<p class="text-xl">Language Model Programs for Embodied Control</p>
		</div>
		<AuthorInfo />
		<AbstractComp />
		<CodeBox :json="json1" />
		<CodeBox :json="json1" />
		<CodeBox :json="json1" />
		<CitationComp />
	</div>
</template>

<script setup>
import AuthorInfo from './components/AuthorInfo.vue'
import AbstractComp from './components/AbstractComp.vue'
import CodeBox from './components/CodeBox.vue'
import CitationComp from './components/CitationComp.vue'
import json1 from './videoData.json'
</script>

<style scoped>
.container {
	width: 96%;
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #212529;
}
@media (min-width: 576px) {
	.container {
		max-width: 540px;
	}
}
@media (min-width: 768px) {
	.container {
		
		max-width: 720px;
	}
}
@media (min-width: 992px) {
	.container {
		max-width: 960px;
	}
}
</style>
