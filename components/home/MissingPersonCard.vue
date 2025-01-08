<template>
    <div class="cardHolder">
        <NuxtLink to="/missingPerson/1" class="image">
            <img src="" alt="">
        </NuxtLink>
        <div class="text">
            <div class="top">
                <div class="name">
                    <span class="mediumText">Name</span>
                    <span>Age: Gender: </span>
                </div>
                <div class="status">

                </div>              
            </div>

            <div class="details">
                <span class="">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur at neque cupiditate debitis illo qui excepturi! Porro, neque magnam eos, omnis eum quas nisi quasi quaerat vero debitis dignissimos sequi!</span>
            </div>

        </div>
    </div>

</template>

<script setup>

</script>

<style scoped>
.cardHolder{
    width: 32%;
    height: 500px;
    border-radius: 20px;
    padding-top:5px;
    padding-left: 5px;
    padding-right:5px;
    padding-bottom:10px;
    margin: 5px;
    border: 1px solid var(--amberalert-text);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.image{
    height: 70%;
    width: 100%;
    background-color: blueviolet;
    border-radius: 20px;
}
.text{
    display: flex;
    flex-direction: column;
    height:30%;
    width: 90%;
    padding-left: 1%;
    padding-right: 1%;
}
.top{
    height: 40%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.name{
    display: flex;
    flex-direction: column;
    width: 70%;
}

.status{
    width: 30px;
    height: 30px;
    background-color: var(--amberalert-green);
    border-radius: 50%;
}
.details{
    height: 60%;
    width: 100%;
    overflow: hidden;
}
</style>