<template>
	<div class="card mb-4 mt-4 text-left border-solid border border-slate-500">
		<h5 class=" card-header text-xl ledaing-10 ">{{ json.name }} </h5>
		<div class="card-body p-4">
			<p class="my-4">Choose a command:</p>
			<select class="form-select" size="5" aria-label="size 5 select example">
				<option v-for="option in json.options" :key="option.key" :value="option.key">
					{{option.name}}
				</option>
			</select>

			<div class="col-md-12 mb-2">
				<video id="vid_fbp" width="100%" preload="metadata" playsinline="" controls="">
					<source src="./../../static/videos/fruits_and_bottles.mp4" type="video/mp4">
				</video>
			</div>

			<div class="row" id="content_fbp_1">
				<div class="col-md-12" id="code_fbp_1">
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	props: { json: Object }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card {
	position: relative;
	display: flex;
	flex-direction: column;
	min-width: 0;
	word-wrap: break-word;
	background-color: #fff;
	background-clip: border-box;
	border: 1px solid rgba(0, 0, 0, .125);
	border-radius: .25rem;
}

.card-header {
	padding: .5rem 1rem;
	margin-bottom: 0;
	background-color: rgba(0, 0, 0, .03);
	border-bottom: 1px solid rgba(0, 0, 0, .125);
}

.card-body {
	flex: 1 1 auto;
	padding: 1rem 1rem;
}
</style>
