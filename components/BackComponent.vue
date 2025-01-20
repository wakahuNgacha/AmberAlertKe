<template>
    <div class="backholder">
        <div class="back" @click="goBack">
            <UIcon name="i-ic:baseline-arrow-back" class="icon"/>
        </div>
    </div>
</template>

<script setup>
const goBack = () => {
    window.history.back(); // This uses the browser's history API to go back
};
</script>

<style scoped>
.backhoder{
    /* height:100px; */
    width: 100%;
    display: flex;
    justify-content: start;
    /* padding-left: 20px;
    padding-right: 20px;
    padding-top: 10px; */
}
.back{
    /* background-color: blue; */
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 10px;
    cursor: pointer;
}
</style>
