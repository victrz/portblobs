<template>
  <div id="app">
		<div class="wrap">
			<div id="header" >
				<h1>Victoria Trzcianowski</h1>
				<h2>Web Developer</h2>
				<img class="black-dots-small desktop-only" src="black6.png">
			</div>
			<div id="top-grid">
				<div class="top-grid-items">
					<div class="each-item w-100 flex just-cont-end loc-blob">
						<div class="each-item-inner blob-1">
							<i class="blob-fa fa fa-map-marker fa-5x" style="color: black;" aria-hidden="true"></i>
							<p class="blob-1-text">Toronto, Ontario<br> Canada</p>
						</div>
					</div>
					<div class="each-item w-100 flex just-cont-end">
						<div class="each-item-inner blob-2">
							<i class="blob-fa-2 fa fa-graduation-cap fa-5x" style="color: black;" aria-hidden="true"></i>
							<p class="blob-2-text">Structural<br> Engineering, <br>Web Development</p>
						</div>
					</div>
				</div>
				<div id="desktop-line-bg">
					<div class="blob-black-1"></div>
				</div>
			</div>
			<div id="mid-grid" class="w-100">
				<div class="each-item first-blob">
					<div class="each-item-inner blob-3 flex-reverse">
						<i class="blob-fa-3 fa fa-keyboard-o fa-5x" style="color: black;" aria-hidden="true"></i>
						<p class="blob-3-text">HTML, CSS, SCSS, <br>JavaScript, Vue.js, PHP,<br> ES2016, angular, wordpress</p>
					</div>
				</div>
				<div class="each-item middle-blob">
					<div class="each-item-inner blob-4">
						<i class="fa fa-heart-o fa-5x" style="color: black;" aria-hidden="true"></i>
						<p class="blob-4-text">Coffee, travel, music, mysteries, celebrity<br> gossip</p>
					</div>
				</div>
				<div class="desktop-only each-item">
					<div class="each-item-inner">
						<img class="black-dots" src="black4.png">
					</div>
				</div>
				<div class="each-item blob-5">
					<div class="each-item-inner flex-reverse">
						<i class="blob-fa-5 fa fa-coffee fa-5x" style="color: black;" aria-hidden="true"></i>
						<p class="blob-5-text">Americano,<br> tea</p>
					</div>
				</div>
			</div>
			<div id="footer">
				<div class="flex contact">
					<div class="flex">
						<a href="mailto:vtrzcianowski@gmail.com?Subject=Web%20Development" target="_top"><i class="fa fa-envelope fa-3x " aria-hidden="false" label="link to send me an email"></i></a>
					</div>
					<div class="flex">
						<a href="https://www.linkedin.com/in/victoria-trzcianowski/"><i class="fa fa-linkedin fa-3x " aria-hidden="false" label="link to my linked in page"></i></a>
					</div>
				</div>
				<div class="desktop-only blob-6">
					<img class="black-dots-small" src="black2.png">
				</div>
			</div>
		</div>
	</div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App'
}
</script>

<style>

body{
	margin:0;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
	background-color: #f8e6d8;
	font-family: 'Playfair Display', serif;
	font-size: 1em;
	text-transform: lowercase;
}
@media only screen and (max-width: 600px) {
	#app {
		background-image: url('/mobileback.png');
		background-repeat: repeat-y;
		background-size: contain;
		background-position: top center;
	}
}
#header{
	width: 100%;
	background-image: url('/headerblob.png');
	background-position: top;
	background-repeat: no-repeat;
	background-size: contain;
	text-align: center;
	padding-bottom: 75px;
	position:relative;
}
#header > img{
	position:absolute;
	top: 5px;
	left: 10%;
}
p{
	font-size: 1em;
}
a{
	color: black;
	align-self: flex-end;
}
a:hover{
	color: black;
}
a:visited{
	color: black;

}
.wrap{
	width: 100%;
	display: flex;
	flex-direction: column;
	margin: auto;
	align-items: center;
}
.flex{
	display: flex;
}
.flex-col{
	flex-direction: column;
}

h1{
	font-size: 2em;
	margin-bottom: 10px;
	margin-top: 10px;
}
@media only screen and (max-width: 650px) {
	h1{font-size: 1.5em;}
}
h2 {
	font-size: 1.2em;
	margin: 0;
}
#top-grid{
	width: 100%;
	margin: auto;
	display: flex;
	background-repeat: no-repeat;
	background-size: 50%;
}
.top-grid-items{
	width: 50%;
	min-width: 300px;
	display: flex;
	flex-direction: column;
}
@media only screen and (max-width: 600px) {
	.top-grid-items{
		margin: auto;
		width: 100%;
	}
}
#mid-grid{
	display: flex;
	flex-wrap: wrap;
	max-width: 600px;
	margin: auto;
	background-image: url('/black2.png');
	background-repeat: no-repeat;
	background-size: 20%;
	background-position: left;
}
@media only screen and (max-width: 600px) {
	#mid-grid{
		flex-direction: column;
		background:none;
	}
}
#footer{
	display: flex;
	width: 100%;
	margin-top: -20px;
}
.contact{
	background-image: url('/footerblob.png');
	background-repeat: no-repeat;
	background-size: cover;
	background-position: top left;
	flex-grow: 1;
	justify-content: center;
	padding-right: 60px;
}
@media only screen and (max-width: 900px) {
	.contact{
		padding-right: 0px;
	}
}
.each-item{
	width: 50%;
}
.blob-1{
	background-image: url('/blob1.png');
	background-repeat: no-repeat;
	background-size: cover;
}
.blob-1-text{
	position: absolute;
	top: 45%;
	right: 20%;
}
.blob-2{
	background-image: url('/blob2.png');
	background-repeat: no-repeat;
	background-size: 60%;
}
.blob-2-text{
	position: absolute;
	bottom: 45%;
	left: 15%;
}
.blob-3{
	background-image: url('/blob3.png');
	background-repeat: no-repeat;
	background-size: cover;
}
.blob-3-text{
	position: absolute;
	top: 35%;
	left: 35%;
}
.blob-4{
	background-image: url('/blob4.png');
	background-repeat: no-repeat;
	background-size: 100%;
}
.blob-4-text{
	position: absolute;
	top: 30%;
	left: 30%;
}
.blob-5{
	background-image: url('/blob5.png');
	background-repeat: no-repeat;
	background-size: contain;
}
@media only screen and (max-width: 900px) {
	.blob-5{
		margin-top: 75px;
		margin-left: 30%;
	}
}

.blob-5-text{
	position: absolute;
	top: 20%;
	left: 30%;
}
.blob-fa{
	position:absolute;
	left: 30%;
	top: 10%;
}
.blob-fa-3{
	position:absolute;
	left: 30%;
}
.blob-fa-2{
	position:absolute;
	left: 0%;
	top: 45%;
}
.blob-fa-5{
	position:absolute;
	top: 30%;
	right: 0;
}
.blob-6{
	width: 300px;
	height: 200px;
	background-repeat: no-repeat;
	background-size: cover;
}
.w-100{
	width: 100%;
}
.just-cont-end{
	justify-content: flex-end;
}
.each-item-inner{
	width: 280px;
	height: 300px;
	position: relative;
}
.fa{
	padding: 30px;
}
.flex-reverse{
	flex-direction: row-reverse;
}
#desktop-line-bg{
	width: 50%;
	background-image: url('/black7.png');
	background-repeat: no-repeat;
	background-size: contain;
}
@media only screen and (max-width: 600px) {
	#desktop-line-bg{
		display: none;
	}
}
.blob-black-1{
	height: 400px;
	width: 300px;
}
.black-dots{
	position: absolute;
	height: 500px;
	left: -70%;
	top: -100%;
}
.black-dots-small{
	height: 200px;
	width: 200px;
}

@media only screen and (max-width: 900px) {
	.desktop-only{display: none;}
}
@media only screen and (max-width: 600px) {
	.first-blob{
		margin: auto;
	}
	.blob-5{
		margin-top: 0;
		margin-left: 0;
	}
	.blob-4{
		margin-left: 30%;
	}
	.each-item{
		width: 100%;
	}
	.loc-blob{
		justify-content: flex-start;
	}
}
@media only screen and (max-width: 500px) {
	.blob-4{
		margin: 75px auto 0 auto;
	}
}
</style>
