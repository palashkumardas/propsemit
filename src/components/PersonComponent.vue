<script setup>
defineProps(["data"]);
</script>

<template>
        <h2 class="text-xl">Child</h2>
        {{ data.name }} is {{ data.age }} years old and live in {{ data.address }}.

    <form action="" class="flex flex-col">
        <label for="name">Name</label>
        <input type="text" name="name" id="name" v-model="data.name">
        <label for="age">Age</label>
        <input type="number" name="age" id="age" v-model="data.age">
        <label for="occupation">Address</label>
        <input type="text" name="occupation" id="occupation" v-model="data.address">
    </form>
    
</template>

<style scoped>

</style>