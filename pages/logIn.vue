<template>
    <div class="holder">
        <div class="left">
            <div class="imageBox">
                <img src="~/assets/images/team.jpg" alt="">
            </div>
        </div>
        <div class="right">
            <div class="form">
                <span class="mediumText">Log in</span>
                <form action="">
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
                            Log in
                        </button>
                    </div>
                </form>
                <span class="normalText"> Dont have an account yet? <NuxtLink to="/signUp" class="highlight">Sign up</NuxtLink></span>
            </div>
        </div>
    </div>
</template>

<script setup>
const config = useRuntimeConfig();
const apiUrl = config.public.API_URL;

const email = ref('')
const password = ref('')

const toast = useToast()

const login = async() =>{
    try{
        const response = fetch(`${apiUrl}/user/`,{
            method: 'POST',
            headers: {
                'Content-Type': 'application/json'
            },
            body: JSON.stringify({
                email: email.value,
                password: password.value,
            })
        })
        if(!response.ok){
            console.log("an error occured")
            toast.add({
                title: 'login up faild',
                description: 'Something went wrong check your inputs and try again',
            })
        }else{
            console.log("success")
            toast.add({
                title: 'login was succesful',
                description: 'Welcome back to amber alert ke',
            })
        }
    }
    catch{
        console.error('Error:', error.message);
    }
}
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
