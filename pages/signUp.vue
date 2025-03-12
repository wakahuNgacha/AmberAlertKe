<template>
    <BackComponent/>
    <div class="holder">
        <div class="left">
            <div class="form">
                <span class="mediumText">Sign Up</span>
                <form action="">
                    <div class="form-group">
                        <label for="firstName" class="normalText">First Name:</label>
                        <input type="text" id="firstName" name="firstName" required>
                    </div>

                    <div class="form-group">
                        <label for="secondName" class="normalText">Second Name:</label>
                        <input type="text" id="secondName" name="secondName" required>
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
                        <label for="password_confirm" class="normalText">Password confirmation:</label>
                        <input type="password" id="password_confirm" name="password_confirm" required>
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
const config = useRuntimeConfig();
const apiUrl = config.public.API_URL;

const firstName = ref('')
const secondName = ref('')
const surName = ref('')
const email = ref('')
const password = ref('')
const password_confirm = ref('')

const toast = useToast()

const signUp = async() => {
    try{
        const response = fetch(`${apiUrl}/user/`,{
            method: 'POST',
            headers: {
                'Content-Type': 'application/json'
            },
            body: JSON.stringify({
                firstName: firstName.value,
                secondName: secondName.value,
                surName: surName.value,
                email: email.value,
                password: password.value,
                password_confirm: password_confirm.value
            })
        })
        if(!response.ok){
            console.log("an error occured")
            toast.add({
                title: 'Sign up faild',
                description: 'Something went wrong check your inputs and try again',
            })
        }else{
            console.log("success")
            toast.add({
                title: 'Signup was succesful',
                description: 'Welcome to amber alert ke',
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
    /* background-color: aqua; */
}

.left {
	width: 50%;
	height: 100%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	text-align: center;
    /* background-color: blueviolet; */
}
.right {
	width: 50%;
	height: 100;
	display: flex;
	justify-content: center;
	align-items: center;
}

.imageBox{
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
	height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
	border-radius: 20px;
	overflow: hidden;
    position: relative;  
    /* background-color: aqua;  */
}
form{
    width: 100%;
    padding: 10px;
}
.form-group {
    margin-bottom: 10px;
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
