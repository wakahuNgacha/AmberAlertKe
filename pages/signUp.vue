<template>
    <div class="holder">
        <div class="left">
            <div class="form">
                <span class="mediumText">Sign Up</span>
                <form action="">
                    <div class="form-group">
                        <label for="name" class="normalText">Name:</label>
                        <input type="text" id="name" name="name" required>
                    </div>

                    <div class="form-group">
                        <label for="email" class="normalText">Email:</label>
                        <input type="email" id="email" name="email" required>
                    </div>

                    <div class="form-group">
                        <label for="password" class="normalText">Password:</label>
                        <input type="password" id="password" name="password" required>
                    </div>

                    <div class="form-group">
                        <button type="submit" class="primaryButton">
                            Sign up
                        </button>
                    </div>
                </form>
                <span class="normalText"> Already a parner? <NuxtLink to="/login" class="highlight">Log in</NuxtLink></span>
            </div>
            
        </div>
        <div class="right">
            <div class="imageBox">
                <img src="~/assets/images/family.jpg" alt="">
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
	align-items: center;
	text-align: center;
}
.right {
	width: 50%;
	height: 100%;
	display: flex;
	justify-content: center;
	align-items: center;
}

.imageBox{
    background-color: blueviolet;
	width: 90%;
	height: 90%;
	border-radius: 20px;
	overflow: hidden;
    position: relative;
}
.imageBox img{
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.form{
	width: 60%;
	height: 90%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: start;
	border-radius: 20px;
	overflow: hidden;
    position: relative;   
}
form{
    width: 100%;
    padding: 10px;
}
.form-group {
    margin-bottom: 15px;
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-items: start;
    width: 100%;
    height: 80px;
    /* background-color: rgb(49, 226, 43);     */
}
.primaryButton{
    width: 100%;
}
/* form label, form input, form button {
    display: block;
    width: 100%;
} */
.highlight{
    color: var(--amberalert-orange);
}
</style>
