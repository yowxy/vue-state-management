<script setup>
 
import { provide, ref } from 'vue';
import Parent from './components/Parent.vue';
const numbers = ref([1,2,3,4,5]);

provide('numbers',numbers);

</script>

<template>
  <main>
    <div>
     <parent :numbers="numbers"/>
    </div>
  </main>
</template>

<style scoped> 


</style>
