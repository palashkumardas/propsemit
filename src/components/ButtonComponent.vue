<script setup>
const props=defineProps(['name','label']);
const emit=defineEmits(['update:name']);

function reverseName(){
    emit('update:name',props.name.split('').reverse().join(''));
}
</script>

<template>
    <!-- <label for="name">{{ name }}</label> -->
    <button @click="reverseName" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded mt-2"> {{label}}</button>
</template>

<style scoped>

</style>