<template>
	<div class="holder">
		<div class="left">
			<div class="heroText">
				<span class="largeText">A Community Bringing Missing Loved Ones Home</span>
				<span class="normalText">
					Amber Alert KE is a Kenyan community-driven platform dedicated to raising public awareness and facilitating the swift recovery of missing children. Our mission is to empower communities to take proactive steps in ensuring the safety and protection of vulnerable children by promoting vigilance, timely reporting, and coordinated action. Through collaborative efforts, verified information sharing, and partnerships with local authorities, we aim to reunite families and provide hope during challenging times. Together, we can create a safer Kenya where every child matters, and no family has to endure the pain of a missing loved one alone.
				</span>		
			</div>

			<div class="callToAction">
				<div class="primaryButton">
					<span>Donate</span>
				</div>
				<div class="secondaryButton">
					<span>Join the Network</span>
				</div>
			</div>
			<div class="callToAction">
				<NuxtLink to="/home" class="primaryButton">
					<span>Missing persons</span>
				</NuxtLink>
			</div>
		</div>

		<div class="right">
			<div class="bigBox">
				<div class="imageBox">
					<img src="~/assets/images/family.jpg" alt="children" />					
				</div>
				<div class="imageText">
					<div class="circle">
						<img class="asterisk" src="~/assets/images/asterisk.png" alt="asterisk">
					</div>
					<div class="imageInfo">
						<span class="smallText">
							This collective vigilance can significantly reduce response times, increase public awareness, and improve the chances of reuniting missing individuals with their families, making communities safer and more connected.
						</span>
					</div>
					<div class="circledText">

					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script setup>

</script>

<style scoped>
.holder {
	width: 100%;
	height: 100vh;
	display: flex;
	padding-left: 20px;
	padding-right: 20px;
}

.left {
	width: 50%;
	height: 100%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	/* align-items: center; */
	text-align: center;
}
.heroText{
	text-align:start;
	display: flex;
	flex-direction: column;
}

.right {
	width: 50%;
	height: 100%;
	display: flex;
	justify-content: end;
	align-items: center;
}

.bigBox {
	height: 90%;
	width: 90%;
	border-radius: 20px;
	background-color: var(--amberalert-darkGreen);
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
}

.imageBox{
	background-color: blueviolet;
	width: 80%;
	height: 60%;
	border-radius: 20px;
	overflow: hidden;
    position: relative;
	/* clip-path: polygon(0% 0%, 100% 0%, 100% 10%, 100% 70%, 70% 100%, 0% 100%); */
}

.imageBox img{
	display: block;
	width: 100%;
	height: 100%;
	object-fit: cover;
    object-position: center;
}

.imageText{
	height: 30%;
	width:80%;
	display: flex;
	align-items: center;
}
.imageText >*{
	margin-right: 20px;
}
.circle{
	display: flex;
	justify-content: center;
	align-items: center;
	width: 90px;
	height: 90px;
	/* padding: 5px; */
	border-radius: 50%;
	background-color: var(--amberalert-green);
	color: var(--amberalert-green);
	margin-bottom: 10px;
}
.imageInfo{
	width: 50%;
	line-height: 1.1;
}
.smallText{
	color: var(--amberalert-white);	
}
.callToAction{
	display: flex;
	width: 100%;
	margin-top: 20px;
}
</style>
