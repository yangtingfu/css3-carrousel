# css3-carrousel
纯css3做的旋转木马
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
		<style>
			*{
				padding: 0;
				margin: 0;
			}
			img{
				width:200px;
				height: 300px;
			}
			body{ background-color: #313131; }
			@keyframes fn{
				0% {transform:rotateX(-15deg) rotateY(0deg);}
			    100%{transform:rotateX(-15deg) rotateY(360deg);}

			}
			@-moz-keyframes fn{
				0% {transform:rotateX(-15deg) rotateY(0deg);}
			    100%{transform:rotateX(-15deg) rotateY(360deg);}
			}
			@-ms-keyframes fn{
				0% {transform:rotateX(-15deg) rotateY(0deg);}
			    100%{transform:rotateX(-15deg) rotateY(360deg);}
			}
			@-webkit-keyframes fn{
				0% {transform:rotateX(-15deg) rotateY(0deg);}
			    100%{transform:rotateX(-15deg) rotateY(360deg);}
			}
			.box{				
		    	width:200px;
            	height:300px;
            	position:relative;
            	margin:auto;
            	margin-top:150px;
            	transform-style:preserve-3d;
            	transform:rotateX(-10deg);
            	animation: fn 10s;
            	animation-iteration-count: infinite;
		    	animation-timing-function: linear;
		    	position: relative
			}
			.box:hover{
				animation-play-state: paused;
			}
			.box>div{
				width:200px;
				height:300px;
				position: absolute;
				left:0;
				top:0;
				
			}
		</style>
	</head>
	<body>
		<div class="box">
			<div style="transform: rotateY(0deg) translateZ(275px);">
				<img src="img/1.png" >
			</div>
			<div style="transform: rotateY(40deg) translateZ(275px);">
				<img src="img/2.png">
			</div>
			<div style="transform: rotateY(80deg) translateZ(275px);">
				<img src="img/3.png">
			</div>
			<div style="transform: rotateY(120deg) translateZ(275px);">
				<img src="img/4.png">
			</div>
			<div style="transform: rotateY(160deg) translateZ(275px);">
				<img src="img/5.png">
			</div>
			<div style="transform: rotateY(200deg) translateZ(275px);">
				<img src="img/6.png">
			</div>
			<div style="transform: rotateY(240deg) translateZ(275px);">
				<img src="img/7.png">
			</div>
			<div style="transform: rotateY(280deg) translateZ(275px);">
				<img src="img/8.png">
			</div>
			<div style="transform: rotateY(320deg) translateZ(275px);">
				<img src="img/9.png" >
			</div>					
		</div>
	</body>
</html>
