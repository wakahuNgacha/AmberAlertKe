<template>
	<div class="holder">
		<div class='left'>
			<span class="largeText">A Community Bringing Missing Loved Ones Home</span>
			<span class="normalText">AmberAlertKE is a Kenyan platform for public alerts on missing children. Our goal is to reunite families through community vigilance and timely action. Together, we can make a difference.</span>
		</div>

		<div class='right'>
			<div class="bigBox">
				<img src="~/assets" alt="children"/>
			</div>
		</div>	
	</div>

</template>

<script setup>
</script>

<style scoped>
.holder{
	widh: 100%;
	height: 100vh;
	display:flex;
}
.left{
	widh: 50%;
	height: 100%;
	display: flex;
	justify-content: center;
	align-items: center;
}
.right{
	widh: 50%;
	height: 100%;
	display: flex;
	justify-content: center;
	align-items: center;
}
.bigBox{
	height:90% ;
	widh: 90% ;
	boderradious: 20px;
	backgroundcolor: var(--amberalert-darkGreen)
}
</style>
