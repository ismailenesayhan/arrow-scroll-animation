``` html
<!-- Model 01 -->
<div class="scrollBox"><span></span><span></span><span></span></div>

<style>
.scrollBox{
	position: absolute;
	top: 135%;
	left: 50%;
	transform: translate(-50%, -50%);
}

.scrollBox span{
	display: block;
	width: 20px;
	height: 20px;
	border-bottom: 2px solid white;
	border-right: 2px solid white;
	transform: rotate(45deg);
	margin: -10px;
	animation: animate 2s infinite;
}
.scrollBox span:nth-child(2){
	animation-delay: -0.2s;
}
.scrollBox span:nth-child(3){
	animation-delay: -0.4s;
}
@keyframes animate{
	0%{
		opacity: 0;
		transform: rotate(45deg) translate(-20px, -20px);
	}
	50%{
		opacity: 1;
	}
	100%{
		opacity: 0;
		transform: rotate(45deg) translate(20px, 20px);
	}
}
</style>

``` 
