<template>
    <div>
        <v-row>
            <v-text-field type="number" label="Monthly Income" v-model.number="inputNumber" placeholder="3218" />
        </v-row>
        <v-row>
            <v-btn class="button" theme="dark" size="large" @click="calculate">Calculate</v-btn>
        </v-row>
        <v-row>
            <v-text-field variant="underlined" class="input" type="text" label="50% Needs" v-model="output50"
                readonly />

            <v-text-field variant="outlined" color="#ffff" class="input" type="text" label="30% Wants" v-model="output30" readonly />

            <v-text-field class="input" type="text" label="20% Saving" v-model="output20" readonly />
        </v-row>
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
.button{
    width: 100%;
    margin-bottom: 20px;
}

.input{
    margin-left: 5px;
    margin-right: 5px;    
}
</style>