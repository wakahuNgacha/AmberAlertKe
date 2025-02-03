<template>
    <div class="fullHolder">
        <div class="formHolder">
            <form action="">
                <div class="form-group">
                    <label for="message">Message:</label>
                    <input type="text" id="message" name="message" required>
                </div>

                <div class="form-group">
                    <button type="submit" class="primaryButton" @click="addMissingPerson">Report Missing Person</button>
                </div> 
            </form>
        </div>        
    </div>

</template>

<script setup>
const config = useRuntimeConfig();
const apiUrl = config.public.API_URL;

const message = ref('')
const missingPerson = ref('');


const toast = useToast()

const addMissingPerson = async() =>{
    try{
        const response = fetch(`${apiUrl}/user/`,{
            method: 'POST',
            headers: {
                'Content-Type': 'application/json'
            },
            body: JSON.stringify({
                message: message.value,
                missingPerson: message.value
            })
        })
        if(!response.ok){
            console.log("an error occured")
            toast.add({
                title: 'Update downloaded.',
                description: 'It will be installed on restart. Restart now?',
            })
        }else{
            console.log("success")
            toast.add({
                title: 'Update downloaded.',
                description: 'It will be installed on restart. Restart now?',
            })
        }

    }
    catch(error){
        console.error('Error:', error.message);
    }

}
</script>

<style scoped>
.fullHolder{
    width: 98%;
    height: 100vh;
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 5;
    background-color: var(--amberalert-white);
}
.formHolder{
    width: 80%;
    height:90%;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 4;
    padding: 10px;
    border-radius: 20px;
    box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.4);
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
</style>