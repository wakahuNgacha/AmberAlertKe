<template>
    <div class="fullholder">
        <div class="formHolder">
            <form action="">
                <div class="form-group">
                            <label for="personName">Person's Name:</label>
                            <input type="text" id="personName" name="personName" required>
                        </div>

                        <div class="form-group">
                            <label for="age">Age:</label>
                            <input type="number" id="age" name="age" required>
                        </div>

                        <div class="form-group">
                            <label for="lastSeen">Last Seen Location:</label>
                            <input type="text" id="lastSeen" name="lastSeen" required>
                        </div>

                        <div class="form-group">
                            <label for="dateMissing">Date Missing:</label>
                            <input type="date" id="dateMissing" name="dateMissing" required>
                        </div>

                        <div class="form-group">
                            <label for="contactInfo">Your Contact Information:</label>
                            <input type="email" id="contactInfo" name="contactInfo" required>
                        </div>

                        <div class="form-group">
                            <button type="submit" class="primaryButton">Report Missing Person</button>
                        </div> 
            </form>
        </div>        
    </div>

</template>

<script setup>
</script>

<style scoped>
.fullHolder{
    width: 100%;
    height: 100vh;
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
}
.formHolder{
    width: 98%;
    height:98%;
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
