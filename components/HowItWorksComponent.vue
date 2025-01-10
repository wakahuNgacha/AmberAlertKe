<template>
	<div class="holder">
		<div class="text">
			<div class="left">
				<div class="circle">
					<img class="asterisk" src="~/assets/images/asterisk.png" alt="asterisk">
				</div>
				<span class="smallText"> The Amber Alert KE system has the potential to create a transformative impact in Kenya by fostering a proactive, community-driven approach to finding missing persons. Through collaboration with local coordinators and leveraging social media platforms like Twitter, WhatsApp, Facebook, and Instagram, the system ensures rapid information sharing and mobilization. </span> 
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
	/* background-color: var(--amberalert-green); */
	padding-left: 20px;
    padding-right: 20px;
	margin-top: 20px;
	height: 100vh;
	display: flex;
	flex-direction: column;
}
.text{
	display: flex;
	/* align-items: center; */
	height: 40%;
	width: 100%;
}
.left{
	width: 40%;
	display: flex;
	flex-direction: column;
	margin-right: 10%;
}
.right{
	width: 40%;
}
.circle{
	display: flex;
	justify-content: center;
	align-items: center;
	width: 60px;
	height: 60px;
	/* padding: 5px; */
	border-radius: 50%;
	background-color: var(--amberalert-green);
	color: var(--amberalert-green);
	margin-bottom: 10px;
}
.right{
	width: 70%;
	justify-content: start;
	align-items: center;
}
.boxHolder{
	display: flex;
	height: 50%
}
.box{
	height: 300px;
	width: 400px;
	margin: 10px;
	border-radius: 20px;
	/* background-color: var(--amberalert-green); */
}
</style>
