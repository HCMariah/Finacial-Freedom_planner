<template>
    <v-col>
        <v-row class="useriput">
            <v-col cols="12" sm="4">
                <h1 style="color: #0CBD6E;">Budget Calculator</h1>
                <v-text-field variant="outlined" color="#0CBD6E" label="Monthly Net Income" v-model.number="inputNumber"
                    placeholder="After Tax Monthly Net Income" prepend-inner-icon="mdi-currency-usd" type="number"
                    hide-spin-buttons />
                <v-btn class="button" theme="dark" width="287px" height="56px" color="#0CBD6E" variant="outlined"
                    @click="calculate">Calculate
                    Budget</v-btn>
            </v-col>
        </v-row>
        <v-row>
            <v-col cols="12" sm="4">
                <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="50% Needs"
                    v-model="output50" prepend-inner-icon="mdi-currency-usd" readonly />
            </v-col>
            <v-col cols="12" sm="4">
                <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="30% Wants"
                    v-model="output30" prepend-inner-icon="mdi-currency-usd" readonly />
            </v-col>
            <v-col cols="12" sm="4">
                <v-text-field variant="outlined" color="#0CBD6E" class="input" type="text" label="20% Saving"
                    v-model="output20" prepend-inner-icon="mdi-currency-usd" readonly />
            </v-col>
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
.useriput {
  justify-content: center;
}
</style>