<template>
    <div class="holder">
        <AddMissingPerson></AddMissingPerson>
        <div class="add">
            <UIcon name="i-ic:outline-plus" class="icon"/>
        </div>
    </div>
</template>

<script setup>
import AddMissingPerson from '~/components/AddMissingPerson.vue';

</script>

<style scoped>
.holder{
    width: 100%;
    height: auto;
    padding-right: 20px;
    padding-left: 20px;
    position: relative;
}
.add{
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 4;
    padding: 10px;
    border-radius: 50%;
    box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.4);
    position: fixed;
    right: 20px;
    bottom: 20px;
    cursor: pointer;
}
</style>
