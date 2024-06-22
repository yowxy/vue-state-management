<script setup>

import Child from './Child.vue';
import useNumbers from '../composables/useNumbers'

const { numbers , addNumbers } = useNumbers();
</script>


<template>
    <div>
        <h1>Parent</h1>
        {{ numbers }}
        <button @click="addNumbers">add</button>
        <div class="line"></div>
        <child />
    </div>
</template>