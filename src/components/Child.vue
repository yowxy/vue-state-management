<script setup>

// import { inject } from 'vue'
import GrandChild from './GrandChild.vue';
import { useNumbers } from '../stores/numbers';

const { numbers, addNumbers } = useNumbers();

// const numbers = inject('numbers');

</script>


<template>
    <div>
        <h1>Child</h1>
        {{ numbers }}
        <button @click="addNumbers">Add</button>
        <div class="line"></div>
        <GrandChild  />
    </div>
</template>