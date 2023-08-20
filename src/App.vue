<script setup>
import { ref,reactive } from 'vue';

// import PersonComponet from './components/PersonComponent.vue';
import SingleItem from './components/SingleItem.vue'; 
// import MultipleComponent from './components/MultipleComponent.vue';
import ButtonComponent from './components/ButtonComponent.vue';

const data=reactive({
  name:'Palash',
  age:30,
  address:'Dhaka'
})
</script>

<template>
  <section class="mx-auto container">
  <h1 class="my-10">Component Model</h1>
    <h2 class="text-xl">Parent</h2>
    {{ data.name }} is {{ data.age }} years old and live in {{ data.address }}
    <!-- <PersonComponet :data="data"/> -->
    <SingleItem v-model="data.name"/> 

    <!-- <MultipleComponent v-model:name="data.name" v-model:age="data.age" v-model:address="data.address"/> -->
    <ButtonComponent v-model:name="data.name" label="Reverse"/>

  </section>
</template>
<style scoped>

</style>
