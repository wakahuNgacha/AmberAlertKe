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
    flex-wrap: wrap; /* Allows items to wrap to the next row if necessary */
    gap: 20px; /* Adds spacing between cards */
    justify-content: space-between; /* Distributes space evenly between cards */
}
</style>
