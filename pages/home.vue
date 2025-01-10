<template>
    <HomeHeader/>
    <div class="holder">
        <HomeMissingPersonCard v-for="i in 5"/>
    </div>

</template>

<script setup>
import MissingPersonCard from '~/components/home/MissingPersonCard.vue';

</script>

<style scoped>
.holder {
    display: flex;
    flex-wrap: wrap;
    padding-right: 20px;
    padding-left: 20px;
    margin-top: 100px;
}
</style>
