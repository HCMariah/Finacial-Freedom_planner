<template>
    <h1 style="color: #0CBD6E;" class="centered">Budget Calculator</h1>
    <v-card color="#192835" class="padding">
        <v-row>
            <v-col>
                <v-text-field variant="outlined" color="#0CBD6E" label="Monthly Net Income" v-model.number="inputNumber"
                    placeholder="Enter Montly Net Income" prepend-inner-icon="mdi-currency-usd" type="number"
                    hide-spin-buttons />
        </v-col>
        <v-col>
            <v-btn class="button" theme="dark" width="100%" size="x-large" color="#0CBD6E" variant="outlined"
                @click="calculate">Calculate
                Budget</v-btn>
        </v-col>
    </v-row>
    <v-row>
        <v-col>
            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="50% Needs"
                v-model="output50" prepend-inner-icon="mdi-currency-usd" readonly />
        </v-col>
        <v-col>
            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="30% Wants"
                v-model="output30" prepend-inner-icon="mdi-currency-usd" readonly />
        </v-col>
        <v-col>
            <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="20% Saving"
                v-model="output20" prepend-inner-icon="mdi-currency-usd" readonly />
        </v-col>
    </v-row>
    </v-card>
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

<style>
.centered {
    justify-content: center;
    display: flex;
    text-align: center;
    margin-bottom: 2rem;
}

.padding {
    padding: 2rem;
    padding-top: 3rem;
}
</style>