<template>
	<div>
		<ul class="author-box mt-8">
			<li><a href="//jacky.io">Jacky Liang</a></li>
			<li><a href="//wenlong.page/">Wenlong Huang</a></li>
			<li><a href="//fxia22.github.io/">Fei Xia</a></li>
			<li>Peng Xu</li>
			<li><a href="//karolhausman.github.io/">Karol Hausman</a></li>
			<li><a href="//brianichter.com/">Brian Ichter</a></li>
			<li><a href="//www.peteflorence.com/">Pete Florence</a></li>
			<li><a href="//andyzeng.github.io/">Andy Zeng</a></li>
			<br>
			<br>
			<li>
				<a href="http://g.co/robotics" class="flex items-center" target="_blank">
					<img src="./../../static/img/robotics-at-google.png" width="40px">
					<span class="ml-2">Robotics at Google</span>
				</a>
			</li>
		</ul>
		<div class="container w-2/5 mx-auto px-4">
			<ul class="link-box grid grid-cols-1 md:grid-cols-3 gap-8">
				<li>
					<a href="https://arxiv.org/abs/2209.07753">
						<div><img src="./../../static/img/paper_small.png" height="60px"></div>

						<h4><strong>Paper</strong></h4>
					</a>
				</li>
				<li>
					<a href="https://github.com/google-research/google-research/tree/master/code_as_policies">
						<div><img src="./../../static/img/github.png" height="60px"></div>
						<h4><strong>Code</strong></h4>
					</a>
				</li>
				<li>
					<a href="https://colab.research.google.com/drive/1V9GU70GQN-Km4qsxYqvR-c0Sgzod19-j">
						<div><img src="./../../static/img/demo.png" height="60px"></div>

						<h4><strong>Demo</strong></h4>
					</a>
				</li>
			</ul>
		</div>

	</div>
</template>

<script>
export default {
	name: 'AuthorInfo',
}
</script>
<style>
.author-box li {
  display: inline-block;
  margin: 0 12px 6px;
}

a {
  color: #1772d0;
  text-decoration: none;
}

.link-box li div {
  width: 45px;
  height: 60px;
  display: table-cell;
  vertical-align: middle;
  text-align: center;
}
</style>
