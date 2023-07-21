<script setup>
import { ref , computed } from 'vue';
let num1 = ref(0);
let num2 = ref(0);
function sumOfnumbers(){
    return Number(num1.value) + Number(num2.value);
}
const sum = computed(() => sumOfnumbers());
</script>

<template>
    <input v-model="num1" type="text" id="number1"><input v-model="num2" type="text" id="number2">
    <label for="number1">Put numbers to display the sum: <span>{{ sum }}</span></label>
    <br>
    <p v-if="sum > 100">This is a big number {{ sum }}</p>
</template>

<style scoped>

</style>
