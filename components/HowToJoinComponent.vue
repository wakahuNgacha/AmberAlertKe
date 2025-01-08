<template>
    <div class="holder">
        <div class="left">
            <div class="bigBox">
                <img src="" alt="anada image">
            </div>
        </div>
        <div class="right">
            <div class="heading">
                <span class="largeText">Amber Alert ke is a Community lead program</span>
            </div>
            <div class="details">
                <span class="smallText">Be part of the movement. Help protect your community by becoming a volunteer, sharing alerts, or supporting our mission. Together, we can make a difference.</span>
            </div>
            <div class="callToAction">
                <div class="public">
                    <span>Want to join the community?</span>
                </div>

                <div class="coordinators">
                    <span>join as a community coordinator</span>
                </div>
            </div>
        </div>

    </div>
</template>

<script setup>
</script>

<style scoped>
.holder{
    width: 100%;
    height: 100vh;
    display: flex;
}
.left{
    width: 50%;
    display: flex;
    justify-content: center;
    align-items:center;
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
.right{
    display: flex;
    flex-direction: column;
}
.heading{
    height:30%;
    width: 100%;
    padding-top: 20px;
    display: flex;
}
.details{
    height: 30%;
    width: 100%;
    padding-top: 20px;
}
.callToAction{
    height: 40%;
    display: flex;

}
.public{
    background-color: var(--amberalert-darkGreen);
}

.coordinators{
    background-color: var(--amberalert-green);
}

</style>