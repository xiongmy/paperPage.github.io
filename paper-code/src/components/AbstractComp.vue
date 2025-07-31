<template>
	<div class="mt-4">
		<video id="v0" width="100%" preload="metadata" playsinline="" muted="" loop="" autoplay="">
			<source src="./../../static/videos/tasks.mp4" type="video/mp4">
		</video>
		<div class="mt-4 text-left">
			<h1 class="text-2xl leading-20">Abstract</h1>
			<p class="text-base leading-6">
				Large language models (LLMs) trained on code-completion have been shown to be capable of synthesizing
				simple
				Python programs from docstrings [1].
				We find that these codewriting LLMs can be re-purposed to write robot policy code, given natural
				language
				commands.
				Specifically, policy code can express functions or feedback loops that process perception outputs
				(e.g.,from
				object detectors [2], [3]) and parameterize control primitive APIs.
				When provided as input several example language commands (formatted as comments) followed by
				corresponding
				policy code (via few-shot prompting), LLMs can take in new commands and autonomously re-compose API
				calls to
				generate new policy code respectively.
				By chaining classic logic structures and referencing third-party libraries (e.g., NumPy, Shapely) to
				perform
				arithmetic, LLMs used in this way can write robot policies that (i) exhibit spatial-geometric reasoning,
				(ii)
				generalize to new instructions, and (iii) prescribe precise values (e.g., velocities) to ambiguous
				descriptions
				(“faster”) depending on context (i.e., behavioral commonsense).
				This paper presents code as policies: a robot-centric formalization of language model generated programs
				(LMPs)
				that can represent reactive policies (e.g., impedance controllers), as well as waypoint-based policies
				(vision-based pick and place, trajectory-based control), demonstrated across multiple real robot
				platforms.
				Central to our approach is prompting hierarchical code-gen (recursively defining undefined functions),
				which can
				write more complex code and also improves state-of-the-art to solve 39.8% of problems on the HumanEval
				[1]
				benchmark.
				Code and videos are available at https://code-as-policies.github.io
			</p>
			<p class="mt-4 text-center">
				<img src="./../../static/img/share_image.png" width="100%">
			</p>
			<div class="mt-4">
				<video id="v0" width="100%" preload="metadata" playsinline="" controls="">
					<source src="./../../static/videos/3_min_explainer.mp4" type="video/mp4">
				</video>
			</div>
			<div class="mt-8 text-left">
				<h3 class="text-2xl leading-20">Experiment Videos and Generated Code</h3>
				<p class="mt-2 text-base leading-6">Videos have sound that showcase voice and speech-based robot
					interface.</p>
				<p class="mt-6 text-base leading-6">Long pauses between commands and responses are mostly caused by
					OpenAI API query times and rate limiting.</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'AbstractComp',
	props: {
		msg: String
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
