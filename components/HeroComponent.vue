<template>
	<div class="holder">
		<div class="left">
			<span class="largeText">A Community Bringing Missing Loved Ones Home</span>
			<span class="normalText">
				AmberAlertKE is a Kenyan platform for public alerts on missing children. Our goal is to reunite families through community vigilance and timely action. Together, we can make a difference.
			</span>
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
/* Fixed spelling errors and syntax issues */
.holder {
	width: 100%; /* Fixed 'widh' to 'width' */
	height: 100vh;
	display: flex;
}

.left {
	width: 50%; /* Fixed 'widh' to 'width' */
	height: 100%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	text-align: center;
	padding: 20px;
}

.right {
	width: 50%; /* Fixed 'widh' to 'width' */
	height: 100%;
	display: flex;
	justify-content: center;
	align-items: center;
}

.bigBox {
	height: 90%;
	width: 90%; /* Fixed 'widh' to 'width' */
	border-radius: 20px; /* Fixed 'boderradious' to 'border-radius' */
	background-color: var(--amberalert-darkGreen); /* Fixed 'backgroundcolor' to 'background-color' */
	display: flex;
	justify-content: center;
	align-items: center;
}

.largeText {
	font-size: 2rem;
	font-weight: bold;
	margin-bottom: 1rem;
}

.normalText {
	font-size: 1rem;
	color: #555;
	line-height: 1.5;
}
</style>

