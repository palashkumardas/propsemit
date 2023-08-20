<script setup>
defineProps(['name','age','address']);
defineEmits(['update:name','update:age','update:address']);
</script>

<template>
    <form action="" class="flex flex-col">
        <label for="name">Name</label>
        <input type="text" name="name" id="name" :value="name" @input="$emit('update:name', $event.target.value)">
        <label for="age">Age</label>
        <input type="number" name="age" id="age" :value="age" @input="$emit('update:age', $event.target.value)">
        <label for="occupation">Address</label>
        <input type="text" name="occupation" id="occupation" :value="address" @input="$emit('update:address', $event.target.value)">
       
    </form>
</template>

<style scoped>

</style>