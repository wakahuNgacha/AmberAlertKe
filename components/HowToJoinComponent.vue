<template>
    <div class="holder">
        <div class="left">
            <div class="bigBox">
                <div class="imageBox">
                    <img src="~/assets/images/team.jpg" alt="a community">
                </div>
                
            </div>
        </div>
        <div class="right">
            <div class="heading">
                <span class="largeText">Amber Alert ke is a Community lead program</span>
            </div>
            <div class="details">
                <span class="normalText">Be part of the movement. Help protect your community by becoming a volunteer, sharing alerts, or supporting our mission. Together, we can make a difference.</span>
            </div>
            <div class="callToAction">
                <div class="public">
                    <div class="pics">
                        <UAvatarGroup size="sm" :max="6">
                            <UAvatar
                            src="https://avatars.githubusercontent.com/u/739984?v=4"
                            alt="benjamincanac"
                            />
                            <UAvatar
                            src="https://avatars.githubusercontent.com/u/904724?v=4"
                            alt="Atinux"
                            />
                            <UAvatar
                            src="https://avatars.githubusercontent.com/u/7547335?v=4"
                            alt="smarroufin"
                            />
                        </UAvatarGroup>
                    </div>
                    <span class="normalText">Be part a community coordinator</span>
                    <div class="bottom">
                        <span>Want to join the community?</span>
                        <div class="arrow">
                            <UIcon name="i-ic:baseline-arrow-outward"/>
                        </div>	                        
                    </div>

                </div>

                <div class="coordinators">
                    <img class="asterisk" src="~/assets/images/asterisk.png" alt="asterisk">
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
.right{
    display: flex;
    justify-content: center;
    width: 50%;
    flex-direction: column;
    padding:20px;
}
.heading{
    height:40%;
    width: 70%;
    display: flex;
}
.details{
    height: 30%;
    width: 40%;
    padding-top: 20px;
}
.callToAction{
    height: 40%;
    display: flex;
}
.public{
    background-color: var(--amberalert-orange);
    width: 40%;
    height: 170px;
    border-radius: 50px;
    display: flex;
    padding: 30px;
    flex-direction: column;
    justify-content: space-between;
    margin-right: 5px;
}
.asterisk{
    width: 50px;
    height: 50px;
}
.bottom{
    display: flex;
    justify-content: space-between;
    align-items: baseline;
}
.coordinators{
    background-color: var(--amberalert-green);
    width: 40%;
    height:170px;
    border-radius: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.arrow{
	width: 30px;
	height: 30px;
	background-color: var(--amberalert-white);
	display: flex;
	justify-content: center;
	align-items: center;
	border-radius: 50%;
}
</style>