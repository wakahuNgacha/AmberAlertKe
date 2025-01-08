<template>
    <HomeHeader/>
    <div class="holder">
        <HomeMissingPersonCard v-for="i in 5"/>
    </div>

</template>

<script setup>
import MissingPersonCard from '~/components/home/MissingPersonCard.vue';

</script>

<style>
</style>
