<template>
	<div>
		<div id="fullpage" class="site__header">
			<div class="section bg1">
				<image class="joinus animated" src="/static/nssolapp/staticsources/joinus.png" data-show="fadeInDown" data-hide="fadeOut"></image>
				<div class="section-main flex flex-v flex-align-center">
					<p class="p1 animated" data-show="fadeInDown" data-delay="100">日铁软件 校园招聘</p>
					<p class="p2 animated" data-show="fadeIn" data-delay="700">欢迎2021届新同学</p>
					<div class="bb flex flex-v flex-pack-center redbg animated" data-show="fadeInUp" data-hide="fadeInDown">
						<p class="p3 animated" data-show="fadeInDown" data-delay="750" data-hide="fadeOutRight">从日铁开始人生新篇章</p>
						<image class="joinusup" src="../../static/nssolapp/staticsources/joinusUp.png"></image>

					</div>
				</div>
				<image class="bgimg" src="/static/nssolapp/staticsources/bg.png"></image>
				<image class="jt" src="/static/dowapp/jt.gif"></image>
				<image class="plane animated" src="../../static/nssolapp/staticsources/plane.png" data-show="fadeInRight"></image>
				<image class="coffee animated" src="/static/nssolapp/staticsources/coffee.png" data-show="fadeInDown" data-delay="200"
				 data-hide="fadeOut"></image>
				<image class="ok animated" src="/static/nssolapp/staticsources/ok.png" data-show="fadeInDown" data-hide="fadeOut"
				 data-delay="300"></image>
				<image class="pencil animated" src="../../static/nssolapp/staticsources/pencil.png" data-show="fadeInDown"></image>
			</div>



			<div class="section bg2" style="background-color: #ffbd9b;">
				<div class="section-main flex flex-v flex-align-center" >
					<p class="p1 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">第二页大标题</p>
					<p class="p2 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">这是中标题</p>
					<p class="p3 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">这里可以写很多的东西，能尽情BB，哪怕强力复读也没有问题。这里可以写很多的东西，能尽情BB，哪怕强力复读也没有问题。</p>
				</div>
			</div>



			<div class="section bg3" style="background-color: #ff7878;">
				<div class="section-main flex flex-v flex-align-center" >
					<p class="p1 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">第三页大标题</p>
					<p class="p2 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">这是中标题</p>
					<p class="p3 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">这里可以写很多的东西，能尽情BB，哪怕强力复读也没有问题。这里可以写很多的东西，能尽情BB，哪怕强力复读也没有问题。</p>
				
				</div>
			</div>




			<div class="section bg4"  style="background-color: #4CD964;">
				<div class="section-main flex flex-v flex-align-center" >
					<p class="p1 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">第四页大标题</p>
					<p class="p2 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">这是中标题</p>
					<p class="p3 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">这里可以写很多的东西，能尽情BB，哪怕强力复读也没有问题。这里可以写很多的东西，能尽情BB，哪怕强力复读也没有问题。</p>
					
				</div>
			</div>




			<div class="section bg5">
				<div class="section-main flex flex-v flex-align-center">
					<p class="p1 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">写这个吊东西真是费烟</p>
					<p class="p2 animated" data-show="fadeInDown" data-delay="100" data-hide="fadeOutUp">来根华子</p>
			
				</div>
			</div>
		</div>
	</div>
</template>
// flex布局兼容性写法
// flex：定义布局为盒模型
// flex-v：盒模型垂直布局
// flex-l：盒模型水平布局
// flex-1：子元素占据剩余的空间
// flex-align-center：子元素垂直居中
// flex-pack-center：子元素水平居中
// flex-pack-justify：子元素两端对齐
// border-box：元素padding不影响
// flex-text：按钮文本居中
<script>
	import PhyTouch from '@/util/phy-touch'
	import Transform from '@/util/phy-touch/transform.js'
	import FullPage from '@/util/phy-touch/alloy_touch.full_page.js'
	window.Transform = Transform

	export default {
		data() {
			return {
				phyTouch: null,
			}
		},
		onReady() {
			this.phyTouch = new FullPage('#fullpage', {
				animationEnd: function() {},
				leavePage: function() {},
				beginToPage: function() {}
			})
		}
	}
</script>
<style>
	@import "./index";
	@import "../../static/css/animate.css";
</style>
