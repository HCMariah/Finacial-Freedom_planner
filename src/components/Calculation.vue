<template>
    <v-col>
        <v-row>
            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="number" label="Monthly Income"
                v-model.number="inputNumber" placeholder="$2,300.00" prefix="$" />
        </v-row>
        <v-row>
            <v-btn class="button" theme="dark" size="small" width="100%" color="#0C6718" @click="calculate">Calculate</v-btn>
        </v-row>
        <v-row>
            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="50% Needs" v-model="output50" prefix="$"
                readonly />

            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="30% Wants"
                v-model="output30" prefix="$" readonly />

            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="20% Saving" v-model="output20" prefix="$"
                readonly />
        </v-row>
    </v-col>
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
    }
}

const formatValue = (value) => {
    return value.toFixed(2);
}
</script>

<style scoped>
.button {
    
    margin-bottom: 20px;
}

.input {
    margin-left: 5px;
    margin-right: 5px;
    padding-top: 1rem;

}
</style>