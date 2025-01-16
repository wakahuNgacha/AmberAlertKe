<template>
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
                        <button type="submit" class="">Report Missing Person</button>
                    </div> 
        </form>
    </div>

</template>

<script setup>
</script>

<style scoped>
</style>
