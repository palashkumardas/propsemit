<script setup>
defineProps(["modelValue"]);
// defineEmits(["update:modelValue"]);
</script>

<template>
    <form>
        <label for="">Name:</label>
        <input type="text" name="occupation" id="occupation" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)">
    </form>
</template>

<style scoped>

</style>