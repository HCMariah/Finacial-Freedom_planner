<template>
    <div>
        <div class=field1>
            <label for="inputNumber">Monthly Income : </label>
            <input type="number" v-model.number="inputNumber" placeholder="3218">
            <button @click="calculate">Calculate</button>
        </div>
        <div class="output-container">
            <div class="output-box">
                50% Needs : <input type="text" v-model="output50" readonly>
            </div>
            <div class="output-box">
                30% Wants : <input type="text" v-model="output30" readonly>
            </div>
            <div class="output-box">
                20% Saving : <input type="text" v-model="output20" readonly>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const inputNumber = ref('');
const output50 = ref('');
const output30 = ref('');
const output20 = ref('');

function calculate() {
    const number = parseFloat(inputNumber.value);

    if (!isNaN(number)) {
        output50.value = formatValue(number * 0.5);
        output30.value = formatValue(number * 0.3);
        output20.value = formatValue(number * 0.2);
    } else {
        output50.value = 'Please enter a valid number';
        output30.value = 'Please enter a valid number';
        output20.value = 'Please enter a valid number';
    }
}

const formatValue = (value) => {
    return value.toFixed(2);
}
</script>

<style scoped>
.field1{
    width: 40%;
    display: inline-block;
    justify-content: center;

}

.output-container {
    display: flex;


}

.output-box {
    width: 30%;
    display: inline-block;
    justify-content: center;
    padding-top: 1rem;
}
</style>