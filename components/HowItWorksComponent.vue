<template>
	<div class="holder">
		<div class="text">
			<div class="left">
				<div class="circle">
					<span class="bigText">*</span>
				</div>
				<span class="smallText">Amber alert Ke is a community owned and lead program. We aim to have the community involved so that information on missing persons can be got and ussed as soon as posible</span> 
			</div>
			<div class="right">
				<span class="bigText"> This is how Amber Alert Ke Works </span>
			</div>
		</div>

		<div class="boxHolder">
			<div class="box" id="boxOne">
				<div class="text"></div>
				<div class="image"></div>
				<div class="arrow"></div>
				<div class="callToAction"></div>
			</div>

			<div class="box" id="boxtwo">
				<div class="text"></div>
				<div class="image"></div>
				<div class="arrow"></div>
				<div class="callToAction"></div>
			</div>

			<div class="box" id="boxThree">
				<div class="text"></div>
				<div class="image"></div>
				<div class="arrow"></div>
				<div class="callToAction"></div>
			</div>
		</div
	</div>
</teplate>

<script setup>
const colors = ["#F2865E", "#EEF26D", "#E0A0F2", "#C7F29B"];

function getRandomColor() {
    return colors[Math.floor(Math.random() * colors.length)];
}

window.onload = function() {
    const boxes = document.querySelectorAll('.box');
    boxes.forEach(box => {
        box.style.backgroundColor = getRandomColor();
    });
}
</script>

<style scoped>
.holder{
	width: 100%;
	padding-left: 10px;
    padding-right: 10px;
	height: 100vh;
	display: flex;
}
.text{
	display: flex;
	height: 40vw;

}
.left{
	width: 40%;
	display: flex;
	flex-direction: column;
	padding-right: 10%;
}
.circle{
	display: flex;
	justify-content: center;
	align-items: center;
	width: fit-content;
	height: fit-content;
	padding; 20px;
	border-radius: 50%;
	background-color: var(amberalert-darkGreen);
	color: var(--amberalert-green);
	margin-bottom: 10px;
}
.right{
	width: 70%;
}
.box{
	height: 200px;
	width: 32%;
	border-radius: 20px;
}
</style>
