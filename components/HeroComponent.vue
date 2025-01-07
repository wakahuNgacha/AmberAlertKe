<template>
	<div class="holder">
		<div class="left">
			<div class="heroText">
				<span class="largeText">A Community Bringing Missing Loved Ones Home</span>
				<span class="normalText">
					AmberAlertKE is a Kenyan platform for public alerts on missing children. Our goal is to reunite families through community vigilance and timely action. Together, we can make a difference.
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
		</div>

		<div class="right">
			<div class="bigBox">
				<img src="" alt="children" />
			</div>
		</div>
	</div>
</template>

<script setup>
// No script content needed yet
</script>

<style scoped>
.holder {
	width: 100%;
	height: 100vh;
	display: flex;
}

.left {
	width: 50%;
	height: 100%;
	display: flex;
	flex-direction: column;
	padding-left: 20px;
	padding-right: 20px;
	/* justify-content: center; */
	align-items: center;
	text-align: center;
	padding: 20px;
}

.right {
	width: 50%;
	height: 100%;
	display: flex;
	justify-content: center;
	align-items: center;
}

.bigBox {
	height: 90%;
	width: 90%;
	border-radius: 20px;
	background-color: var(--amberalert-darkGreen);
	display: flex;
	justify-content: center;
	align-items: center;
}
</style>
