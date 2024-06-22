<script setup>

import GreatGrandChild from './GreatGrandChild.vue'
import useNumbers from '../composables/useNumbers'

const { numbers , addNumbers } = useNumbers();
</script>


<template>
    <div>
        <h1>GrandChild</h1>
        {{ numbers }}
        <button @click="addNumbers">add</button>
        <div class="line"></div>
        <GreatGrandChild  />
    </div>
</template>