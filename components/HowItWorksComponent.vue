<template>
	<div class="holder">
		<div class="text">
			<div class="left">
				<div class="circle">
					<span class="bigText">*</span>
				</div>
				<span class="smallText">Amber alert Ke is a community owned and led program. We aim to have the community involved so that information on missing persons can be received and used as soon as possible.</span> 
			</div>
			<div class="right">
				<span class="largeText"> This is how Amber Alert Ke Works </span>
			</div>
		</div>

		<div class="boxHolder">
			<div class="box" id="boxOne">
				<div class="text"></div>
				<div class="image"></div>
				<div class="arrow"></div>
				<div class="callToAction"></div>
			</div>

			<div class="box" id="boxTwo">
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
		</div>
	</div>
</template>

<script setup>
const colors = ["#F2865E", "#EEF26D", "#E0A0F2", "#C7F29B"];

function getRandomColor() {
    return colors[Math.floor(Math.random() * colors.length)];
}

function applyRandomColors() {
    const boxes = document.querySelectorAll('.box');
    boxes.forEach(box => {
        box.style.backgroundColor = getRandomColor();
    });
}

onMounted(applyRandomColors);
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
	width: 20px;
	height: 20px;
	padding: 20px;
	border-radius: 50%;
	background-color: var(--amberalert-darkGreen);
	color: var(--amberalert-green);
	margin-bottom: 10px;
}
.right{
	width: 70%;
	justify-content: center;
}
.box{
	height: 200px;
	width: 31%;
	margin: 10px;
	border-radius: 20px;
	background-color: var(--amberalert-green);
}
</style>
